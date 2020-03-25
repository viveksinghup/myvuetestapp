<template>
  <div>
    <section class="header">
      <div class="container">
        <div class="header_box flex flex-between">
          <div>Have any question?</div>
          <div class="header_rightbox">
            <span>
              <img src="../assets/images/msg.png" /> contact@mail.com
            </span>
            <span>
              <img src="../assets/images/call.png" /> +080 0444 333 444
            </span>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <div class="header_menu flex flex-between">
          <div class="header-logo">
            <img src="../assets/logo.png" />
          </div>
          <ul class="header_links">
            <li>About</li>
            <li>Features</li>
            <li>Project</li>
            <li>Pages</li>
            <li>Contact</li>
            <li>
              <img src="../assets/images/search.png" />
            </li>
          </ul>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../assets/css/App.scss";

.header {
	background-color: $gray-10;
  &_box {
    padding: 17px 0px;
    @media screen and (max-width: $screen-width-md) {
      flex-direction: column;
    }
  }
  &_rightbox {
    width: 320px;
    display: flex;
    justify-content: space-between;
    span {
      display: flex;
      align-items: center;
      img {
        width: 15px;
        margin-right: 5px;
      }
    }
  }
  &_menu {
    padding: 26px 0px;
    display: flex;
	align-items: center;
	@media screen and (max-width: $screen-width-md) {
		flex-direction: column;
		align-items: center;
    }
  }
  &_links {
    display: flex;
    li {
      margin-left: 20px;
      cursor: pointer;
      transition: 0.45s;
      &:hover {
        color: $yellow;
      }
    }
  }
}
</style>
