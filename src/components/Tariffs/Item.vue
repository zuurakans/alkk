<template>
  <div class="tariffs-item">
    <TagH className="tariffs__title" type="h5">Продвижение по позициям</TagH>
    <img :src="tariffImg" alt="" />
    <div class="tariffs-item__description">
      Продвинем 10 сылок на первые места
    </div>
    <span class="tariffs-item__price">15000 руб</span>
    <Button className="btn-light" text="Оставить заявку" />
  </div>
</template>

<script>
import TagH from "../TagH/TagH.vue";
import tariffImg from "@/assets/tariffs-item-1.png";
import Button from "../Buttons/Button.vue";
export default {
  components: { TagH, Button },
  data() {
    return {
      tariffImg,
    };
  },
};
</script>

<style>
.tariffs-item__price {
  margin:15px 0 25px 0;
}
.btn-light {
  margin-top: 25px;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 150%;
  color: #000000;

}
.tariffs-item__description{
  padding-bottom:15px;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 21px;
  color: #000000;
}
</style>