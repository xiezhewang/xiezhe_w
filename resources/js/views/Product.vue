<template>
    <!-- Main item container -->
    <main class="item">
      <section class="img">
        <button class="img-main__btnlft img-main__btn">
          <img
            src="images/icon-next.svg"
            alt="next symbol image"
            class="img-main__btnlft-img img-main__btn-img"
          />
        </button>
        <button class="img-main__btnrgt img-main__btn">
          <img
            src="images/icon-next.svg"
            alt="next symbol image"
            class="img-main__btnrgt-img img-main__btn-img"
          />
        </button>
        <img src="images/image-product-1.jpg" alt="" class="img-main" />
        <div class="img-btns">
          <button class="img-btn">
            <img
              src="images/image-product-1.jpg"
              alt="shoe product image"
              class="img-btn__img"
            />
          </button>
          <button class="img-btn">
            <img
              src="images/image-product-2.jpg"
              alt="shoe product image"
              class="img-btn__img"
            />
          </button>
          <button class="img-btn">
            <img
              src="images/image-product-3.jpg"
              alt="shoe product image"
              class="img-btn__img"
            />
          </button>
          <button class="img-btn">
            <img
              src="images/image-product-4.jpg"
              alt="shoe product image"
              class="img-btn__img"
            />
          </button>
        </div>
      </section>

      <section class="price">
        <h1 class="price-main__heading">Fall Limited Edition Sneakers</h1>
        <p class="price-txt">
          These low-profile sneakers are your perfect casual wear companion.
          Featuring a durable rubber outer sole, they’ll withstand everything
          the weather can offer.
        </p>
        <div class="price-box">
          <div class="price-box__main">
            <span class="price-box__main-new">$125.00</span>
            <span class="price-box__main-discount"> 50%</span>
          </div>
          <span class="price-box__old">$250.00</span>
        </div>

        <div class="price-btnbox">
          <div class="price-btns">
            <button class="price-btn__add price-btn">
              <img
                src="images/icon-plus.svg"
                alt="plus sign"
                class="price-btn__add-img price-btn__img"
              />
            </button>
            <span class="price-btn__txt">0</span>
            <button class="price-btn__remove price-btn">
              <img
                src="images/icon-minus.svg"
                alt="minus sign"
                class="price-btn__remove-img price-btn__img"
              />
            </button>
          </div>
          <button class="price-cart__btn btn--orange">
            <img
              src="images/icon-cart.svg"
              alt="cart image"
              class="price-cart__btn-img"
            />
            Add to cart
          </button>
        </div>
      </section>
    </main>



</template>

<script>
export default {
    
}
</script>

<style scoped>
.btn--orange {
  padding: 1.5rem 3rem;
  font-size: 1.5rem;
  font-weight: 700;
  color: hsl(0, 0%, 100%);
  background-color: hsl(26, 100%, 55%);
  border: none;
  border-radius: 1rem;
  cursor: pointer;
}

.head-cart {
  z-index: 100;
  padding: 3rem 2rem;
  width: 36rem;
  box-shadow: 0px 10px 25px 3px rgba(0, 0, 0, 0.5);
  border-radius: 1rem;
  position: absolute;
  top: 15%;
  right: 15%;
  display: flex;
  flex-direction: column;
  gap: 4rem;
  visibility: hidden;
}

.head-cart__heading {
  position: relative;
  font-size: 1.5rem;
}


.head-cart__txt {
  font-size: 1.5rem;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  visibility: hidden;
}

.head-cart__btn {
  align-self: center;
  width: 100%;
}

.head-cart__item-wrapper {
  display: flex;
  align-items: start;
  gap: 2.5rem;
}
.head-cart__item {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  visibility: hidden;
}

.head-cart__item-img {
  width: 5rem;
  height: 5rem;
  border-radius: 0.5rem;
}

.head-cart__item-btn {
  align-self: center;
  background: none;
  border: none;
  cursor: pointer;
}

.head-cart__des {
  flex-shrink: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.head-cart__des-txt {
  font-size: 1.5rem;
  line-height: 1.5;
}

.head-cart__price {
  display: flex;
  gap: 1rem;
  font-size: 1.5rem;
}

.head-cart__price-total {
  font-weight: 700;
}


.item {
  padding: 0 3rem;
  max-width: 134rem;
  margin: auto;
  display: grid;
  grid-template-columns: 0.8fr 1fr;
  gap: 10rem;
}

.img-main {
  margin-top: 3rem;
  max-width: 100%;
  border-radius: 5%;
  cursor: pointer;
  margin-bottom: 3.5rem;
}

.img-main__btn {
  display: none;
}

.img-btns {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 2rem;
}

.img-btn {
  display: block;
  cursor: pointer;
  background: none;
  border: none;
  border-radius: 10%;
  transition: all 0.3s;
  position: relative;
}


.img-btn__img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 10%;
  border: 3px solid transparent;
  transition: all 0.3s;
  transform-origin: bottom;
}

.price {
  margin-top: 2rem;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.price-sub__heading {
  text-transform: uppercase;
  letter-spacing: 1.5px;
  font-size: 1.5rem;
  font-weight: 700;
  color: hsl(26, 100%, 55%);
}

.price-main__heading {
  font-size: 3rem;
  font-weight: 700;
}

.price-txt {
  margin-top: 0.8rem;
  font-size: 1.2rem;
  line-height: 1.5;
}

.price-box {
  display: flex;
  flex-direction: column;
  gap: 1.6rem;
}

.price-box__main {
  display: flex;
  gap: 1rem;
  align-items: center;
}

.price-box__main-new {
  font-size: 2.5rem;
  font-weight: 700;
}

.price-box__main-discount {
  border: none;
  padding: 0.5rem 1.25rem;
  background-color: hsl(25, 100%, 94%);
  border-radius: 0.5rem;
  font-size: 1.7rem;
  font-weight: 700;
  color: hsl(26, 100%, 55%);
}

.price-box__old {
  font-size: 1.5rem;
  color: hsl(220, 14%, 75%);
  position: relative;
  text-decoration: line-through;
}

.price-box__old::after {
  content: "";
  height: 1px;
  width: 9%;
  background-color: hsl(220, 14%, 75%);
  position: absolute;
  left: 0;
  top: 50%;
}

.price-btnbox {
  margin-top: 2rem;
}

.price-btnbox {
  display: flex;
  gap: 2.5rem;
}

.price-btns {
  padding: 1.5rem 1rem;
  border: none;
  background-color: hsl(223, 64%, 98%);
  border-radius: 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 3.5rem;
}

.price-btn {
  border: none;
  background: none;
  cursor: pointer;
  height: 100%;
}

.price-btn__txt {
  font-size: 1.7rem;
  font-weight: 700;
}

.price-cart__btn {
  box-shadow: 0px 10px 25px 3px rgba(255, 125, 26, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1.5rem;
}

</style>
