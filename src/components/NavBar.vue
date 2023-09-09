<template>
  <div class="header__nav">
    <div class="burger__menu">
      <input type="checkbox" id="menu__toggle" />
      <label class="burger__btn" for="menu__toggle">
        <span></span>
      </label>
      <ul class="burger__list">
        <li><a class="burger__text" href="">Home</a></li>
        <li><a class="burger__text" href="">Category</a></li>
        <li><a class="burger__text" href="">About</a></li>
        <li><a class="burger__text" href="">Contact</a></li>
      </ul>
    </div>
    <div class="logo">
      <img src="./../assets/logo/logo.png" alt="" />
    </div>
    <nav>
      <ul class="nav__list">
        <li>
          <a href="#">Home</a>
        </li>
        <li>
          <a href="#">Category</a>
        </li>
        <li>
          <a href="#">About</a>
        </li>
        <li>
          <a href="#">Contact</a>
        </li>
      </ul>
    </nav>
    <div class="nav__input">
      <i
        ><svg
          width="18"
          height="18"
          viewBox="0 0 18 18"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M17.0916 15.9083L14 12.8417C15.2001 11.3454 15.7812 9.44609 15.624 7.53443C15.4667 5.62276 14.583 3.844 13.1546 2.56388C11.7261 1.28377 9.86149 0.599604 7.94408 0.652071C6.02668 0.704538 4.20225 1.48965 2.84593 2.84596C1.48962 4.20228 0.704507 6.02671 0.65204 7.94411C0.599573 9.86152 1.28374 11.7262 2.56385 13.1546C3.84397 14.5831 5.62273 15.4668 7.5344 15.624C9.44606 15.7813 11.3453 15.2001 12.8416 14L15.9083 17.0667C15.9858 17.1448 16.078 17.2068 16.1795 17.2491C16.281 17.2914 16.39 17.3132 16.5 17.3132C16.61 17.3132 16.7189 17.2914 16.8205 17.2491C16.922 17.2068 17.0142 17.1448 17.0916 17.0667C17.2418 16.9113 17.3258 16.7036 17.3258 16.4875C17.3258 16.2714 17.2418 16.0637 17.0916 15.9083ZM8.16665 14C7.01292 14 5.88511 13.6579 4.92582 13.0169C3.96653 12.3759 3.21886 11.4649 2.77735 10.399C2.33584 9.3331 2.22032 8.16021 2.4454 7.02865C2.67048 5.8971 3.22605 4.8577 4.04186 4.04189C4.85766 3.22608 5.89707 2.67051 7.02862 2.44543C8.16018 2.22035 9.33307 2.33587 10.399 2.77738C11.4649 3.21889 12.3759 3.96657 13.0169 4.92585C13.6579 5.88514 14 7.01295 14 8.16668C14 9.71378 13.3854 11.1975 12.2914 12.2915C11.1975 13.3854 9.71374 14 8.16665 14Z"
            fill="#667479"
          />
        </svg>
      </i>
      <input type="text" placeholder="Search something here!" />
    </div>
    <my-button class="adaptive" title="Join the community"></my-button>
    <div class="money__table" @click="openMenu">
      <div class="money__valute">
        <i class="country__icon"></i>
        <span class="money__text">VND</span>
        <i class="money__arrow"></i>
      </div>
      <div class="money__list list__none">
        <div class="valute">
          <img src="./../assets/icons/RUB.png" alt="" />
          RUB
        </div>
        <div class="valute">
          <img src="./../assets/icons/BYN.png" alt="" />
          BYN
        </div>
        <div class="valute">
          <img src="./../assets/icons/USA.png" alt="" />
          USA
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import MyButton from './UI/ButtonBlue.vue';
export default {
  components: {
    MyButton,
  },
  methods: {
    openMenu() {
      document.querySelector('.money__list').classList.toggle('list__none');
      document.querySelector('.money__arrow').classList.toggle('rotate');
    },
    openBurgerMenu() {
      document.querySelector('.burger__menu').classList.toggle('active');
      document.querySelector('.burger__btn').classList.toggle('active');
    },
  },
};
</script>
<style scoped>
.header__nav {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}

.money__table {
  position: relative;
  user-select: none;
}
.money__list {
  position: absolute;
  top: 45px;
  left: 8px;
  background: white;
  border-radius: 15px;
}
.list__none {
  display: none;
}

.valute {
  display: flex;
  gap: 5px;
  padding: 15px 20px;
  cursor: pointer;
}

.valute img {
  width: 100%;
  height: 100%;
}

.logo img {
  vertical-align: middle;
}

.nav__list {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 48px;
  color: var(--primary-color-dark-blue, #003459);
  font-size: 16px;
  font-weight: 700;
  line-height: 24px;
}

.nav__input {
  display: flex;
  justify-content: flex-start;
  padding: 15px;
  align-items: center;
  gap: 12px;
  width: 280px;
  height: 44px;
  border-radius: 52px;
  background-color: white;
}

.nav__input input {
  outline: none;
  width: 200px;
}

.btn__blue {
  display: flex;
  justify-content: center;
  align-items: center;
  padding-right: 18px;
  padding-left: 28px;
  font-size: 16px;
  color: #fdfdfd;
  background-color: #003459;
  height: 44px;
  border-radius: 57px;
}

.money__valute {
  display: flex;
  align-items: center;
  cursor: pointer;
  padding: 10px;
  border-radius: 15px;
  transition: 0.3s ease;
}

.money__valute:hover {
  cursor: pointer;
  background-color: #00345919;
}

.money__text {
  padding-left: 8px;
  padding-right: 4px;
}
.country__icon {
  content: '';
  display: block;
  background: url(../assets/icons/VDN_Valute.svg);
  width: 16px;
  height: 16px;
}

.money__arrow {
  display: block;
  content: '';
  background: url(../assets/icons/arrow_down.svg);
  width: 24px;
  height: 24px;
}

.rotate {
  transform: rotate(180deg);
}
@media(min-width: 850px){
  .burger__menu{
    display: none;
  }
}
@media (max-width: 849px) {
  nav {
    display: none;
  }
  .nav__input {
    display: none;
  }
  .adaptive {
    display: none;
  }
  .money__table {
    display: none;
  }
  .logo {
    margin: 0 auto;
  }

  .burger__btn {
    display: flex;
    align-items: center;
    position: fixed;
    top: 30px;
    left: 15px;
    width: 26px;
    height: 26px;
    cursor: pointer;
    z-index: 1;
  }

  .burger__btn span,
  .burger__btn span::before,
  .burger__btn span::after {
    display: block;
    position: absolute;
    width: 100%;
    height: 2px;
    background-color: #616161;
    transition-duration: 0.3;
  }
  .burger__btn span::before {
    content: '';
    top: -5px;
    transition: all 0.3s;
  }
  .burger__btn span::after {
    content: '';
    top: 5px;
    transition: all 0.3s;
  }

  #menu__toggle:checked ~ .burger__btn > span {
    transform: rotate(45deg);
  }
  #menu__toggle:checked ~ .burger__btn > span::before {
    top: 0;
    transform: rotate(0);
  }
  #menu__toggle:checked ~ .burger__btn > span::after {
    top: 0;
    transform: rotate(90deg);
  }
  #menu__toggle {
    opacity: 0;
  }
  .burger__list {
    display: block;
    position: fixed;
    visibility: hidden;
    top: 0;
    left: -100%;
    width: 300px;
    height: 100%;
    margin: 0;
    padding: 80px 0;
    list-style: none;
    background-color: #eceff1;
    box-shadow: 1px 0px 6px rgba(0, 0, 0, 0.2);
    transition-duration: 0.25s;
  }

  .burger__text{
    display: block;
    padding: 30px 24px;
    color: #333;
    font-size: 20px;
    font-weight: 600;
    text-decoration: none;
    transition-duration: .25s;
  }
  .burger__text:hover {
    background-color: #CFD8DC;
  }
  #menu__toggle:checked ~ .burger__list{
    visibility: visible;
    left: 0;
  }
  #menu__toggle:checked ~ .burger__menu{
    overflow: hidden;
    background-color: gray;
  }
}
</style>
