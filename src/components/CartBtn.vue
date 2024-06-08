<template>
  <div class="cart-btn">
    <Routerlink to="/cart" class="cart">
      <i class="bi bi-cart2"></i>
    </Routerlink>
      <span class="count">3</span>
  </div>
</template>

<script>

</script>

<style>
.cart-btn{
  display: flex;
  align-items: center;
  gap: 10px;
  transition: .5s;
}
.cart{
  font-size: 30px;
  color: #fff;
}
.count{
  font-size: 1.2rem;
  color: #fff;
  width: 30px;
  height: 30px;
  padding: 5px;
  border-radius: 50%;
  background: #00a950;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>