<template>
  <div class="container">
    <main>
      <Logo />
      <div class="title-block">
        <h2 class="title title-subhead">Glimp Co. Field Guides</h2>
        <h1 class="title">Girl Scout Cookies</h1>
        <h1 class="title title-emphasis">Ranked</h1>
      </div>
      <p class="site-description">
        Time to buy Girl Scout cookies but not sure which ones to get? Let this
        kinda-definitive ranking be your guide!
      </p>
      <!-- <p class="site-description">
        Ten participants blind-tasted and rated Girl Scout cookies from both
        Little Brownie Bakers and ABC Bakers on taste, texture, and
        snackability, and I crunched the numbers to see which cookies reign
        supreme.
      </p> -->
      <p class="site-description">
        View cookies by bakery, or see how the bakeries' offerings compare to
        one another with Bakery Face-Off. It's better snacking through science!
      </p>
      <ul class="main-link-buttons">
        <li><a href="/abc">ABC Bakers</a></li>
        <li><a href="/lbb">Little Brownie Bakers</a></li>
        <li><a href="/face-off">Bakery Face-Off</a></li>
      </ul>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "assets/global_variables";
@import "assets/main";

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
  max-width: 1440px;
}

.title-block {
  margin: auto;
  margin-top: 2rem;
  margin-bottom: 2rem;
}

.title {
  font-weight: $bold;
  display: block;
  font-size: 3.5rem;
  line-height: 1;
  margin-top: 0;
  margin-bottom: 0;
}

.title-subhead {
  font-size: 1rem;
  margin-bottom: 0.5em;
  line-height: 1;
  text-transform: uppercase;
  letter-spacing: $wide;
}

.title-emphasis {
  font-family: $hand;
  font-weight: $normal;
  color: $winner;
  letter-spacing: $close;
  transform: skewY(-10deg);
}

.site-description {
  font-weight: $normal;
  font-size: 1.2rem;
  line-height: 1.25;
  max-width: 70ch;
  margin-left: auto;
  margin-right: auto;
}

.main-link-buttons {
  list-style-type: none;
  margin: 1.5rem auto;
  padding: 0;
}

.main-link-buttons li a {
  display: block;
  flex-grow: 1;
  font-size: 1.2rem;
  line-height: 1;
  max-width: 30ch;
  margin: 0.35em auto;
  padding: $buttonPadding;
  border-radius: $buttonBorderRadius;
  background: $buttonBg;
  color: $buttonText;
  text-decoration: none;
  transition: background 0.25s ease-in-out;
}

.main-link-buttons li a:hover {
  background: $buttonBgHover;
}

@media only screen and (min-width: 600px) {
  .main-link-buttons {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .main-link-buttons li a {
    display: inline-block;
    flex-grow: 1;
    font-size: 1.2rem;
    margin: 0.35em;
  }
}

@media only screen and (max-width: 400px) {
  .title {
    font-size: 2rem;
  }

  .title-subhead {
    font-size: 0.75rem;
  }

  .title-emphasis {
    font-size: 2.75rem;
  }
}
</style>
