<template>
  <section class="products">
    <div class="container">
      <div class="products-wrapper" id="goods-container">
        <div class="products-card" v-for="item in goodsArray" :key="item.id">
          <div class="products-card___image">
            <img :src="getUrl(item.image)" :alt="item.alt || item.title" />
          </div>
          <div class="products-card__description">
            <div class="products-card__description-row">
              <h5 class="products-card__description--name">
                {{ item.title }}
              </h5>
            </div>
            <div class="products-card__description-row">
              <p class="products-card__description--text">
                {{ item.description }}
              </p>
            </div>
            <div class="products-card__description-row">
              <div class="products-card__description-controls">
                <button class="btn primary">
                  В корзину
                  <img
                    src="../assets/images/items/cart-min.svg"
                    alt="cart-min"
                  />
                </button>
                <span class="products-card__description-controls--price"
                  >{{ item.price }} ₽</span
                >
              </div>
            </div>
          </div>
        </div>
        <!--        ===-->
      </div>
    </div>
  </section>
</template>

<script setup>
import { goodsArray } from "@/constants/goods.js";

const getUrl = (name) => {
  return new URL(`../assets/images/goods/${name}`, import.meta.url);
};
</script>
