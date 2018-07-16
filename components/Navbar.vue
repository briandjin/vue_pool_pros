<template>
<header>
  <nav class="nav--top">
    <div class="row">
      <a href="/">Dealers and Distributors</a>
      <a href="/">Commercial Services</a>
      <i>
        <img src="../assets/images/action-commercial-icon.png" alt="">
      </i>
    </div>
  </nav>
  <nav class="nav--bottom">
    <div class="row">
      <div class="logo-wrapper">
        <img src="../assets/images/pool-pros-logo.png" alt="">
      </div>
      <div class="menu--options">
        <a href="/">Pools &amp; Spas</a>
        <a href="/">Supplies</a>
        <a href="/">Resources</a>
        <a href="/">Services</a>
        <button>Find a Pool Pro</button>
      </div>
    </div>
  </nav>
</header>
</template>
<script>
export default {
  name: 'Navbar'
}
</script>
<style lang="scss" scoped>
@import "../layouts/scss/_variables";

.row {
    width: 90%;
    display: flex;
}

header {
    box-shadow: 0 3px 3px -2px $color--lightgrey;

    a {
        text-decoration: none;
    }

    nav {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .nav {
        &--bottom {
            height: 100px;

            a {
                color: $color--darkblue;
                font-family: Semibold;
                font-size: 14px;
            }

            button {
                display: flex;
                align-items: center;
                justify-content: center;
                width: 150px;
                height: 40px;
                font-family: Semibold;
                font-size: 14px;
                background-color: white;
                border: 1px solid #216CDF;
                color: #216CDF;
                border-radius: 4px;
                outline: none;
            }

            .logo-wrapper {
                flex: 1;

                img {
                    width: 43.96%;
                    height: auto;
                }
            }

            .row {
                justify-content: space-between;
            }

            .menu--options {
                display: flex;
                flex: 1;
                justify-content: space-between;
                align-items: center;

                a {
                  display: flex;
                }
            }
        }

        &--top {
            height: 40px;
            background-color: $color--darkblue;

            a {
                color: $color--white;
                display: flex;
                font-size: 14px;
                font-family: Regular;
                text-align: center;
                margin-left: 3%;
            }

            i img {
                width: 14px;
                margin: 3px 0 0 10px;
            }

            .row {
                justify-content: flex-end;
            }
        } // nav.__navbar--top

    } // nav.navbar
} // header
</style>

