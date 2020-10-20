<template>
  <div class="_container">
    <button
      type="hidden"
      data-toggle="modal"
      data-target="#exampleModal"
      ref="xnxnxnx"
      style="display: none"
    ></button>
    <div class="_head_container">
      <div class="_head_left">
        <div class="_head_left_logo" @click="setMode('congratulation')">BC</div>
        <div class="_head_left_text">Boldseams Couture</div>
      </div>
      <div class="_head_right">
        <div class="_head_right_logo">
          <svg
            width="30px"
            height="30px"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 448 512"
            class="svg-inline--fa fa-bell fa-w-14 fa-3x"
          >
            <path
              fill="currentColor"
              d="M224 480c-17.66 0-32-14.38-32-32.03h-32c0 35.31 28.72 64.03 64 64.03s64-28.72 64-64.03h-32c0 17.65-14.34 32.03-32 32.03zm209.38-145.19c-27.96-26.62-49.34-54.48-49.34-148.91 0-79.59-63.39-144.5-144.04-152.35V16c0-8.84-7.16-16-16-16s-16 7.16-16 16v17.56C127.35 41.41 63.96 106.31 63.96 185.9c0 94.42-21.39 122.29-49.35 148.91-13.97 13.3-18.38 33.41-11.25 51.23C10.64 404.24 28.16 416 48 416h352c19.84 0 37.36-11.77 44.64-29.97 7.13-17.82 2.71-37.92-11.26-51.22zM400 384H48c-14.23 0-21.34-16.47-11.32-26.01 34.86-33.19 59.28-70.34 59.28-172.08C95.96 118.53 153.23 64 224 64c70.76 0 128.04 54.52 128.04 121.9 0 101.35 24.21 138.7 59.28 172.08C421.38 367.57 414.17 384 400 384z"
              class=""
            ></path>
          </svg>
          <span class="_head_count">6</span>
        </div>
        <div class="_head_right_text">
          <span>Godwin Daniel</span>
          <a href="javascript:void(0)">Log Out</a>
        </div>
      </div>
    </div>
    <div class="_body_container">
      <div class="_side_bar"></div>
      <div class="_main_content">
        <div class="_main_bread_crom">
          <div class="_bread_left">
            <div class="_bread_first">
              <div class="_bread_item">Settings</div>
            </div>
            <div class="_bread_second">
              <div class="_bread_item_2">User and Business Profiles</div>
            </div>
          </div>
          <div class="_bread_right">
            <div class="icon_wrap">
              <svg
                width="20px"
                height="20px"
                role="img"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 512 512"
                class="svg-inline--fa fa-exclamation-circle fa-w-16 fa-2x"
              >
                <path
                  stroke-width="2"
                  fill="currentColor"
                  d="M256 40c118.621 0 216 96.075 216 216 0 119.291-96.61 216-216 216-119.244 0-216-96.562-216-216 0-119.203 96.602-216 216-216m0-32C119.043 8 8 119.083 8 256c0 136.997 111.043 248 248 248s248-111.003 248-248C504 119.083 392.957 8 256 8zm-11.49 120h22.979c6.823 0 12.274 5.682 11.99 12.5l-7 168c-.268 6.428-5.556 11.5-11.99 11.5h-8.979c-6.433 0-11.722-5.073-11.99-11.5l-7-168c-.283-6.818 5.167-12.5 11.99-12.5zM256 340c-15.464 0-28 12.536-28 28s12.536 28 28 28 28-12.536 28-28-12.536-28-28-28z"
                  class=""
                ></path>
              </svg>
            </div>
          </div>
        </div>
        <section class="_main_content_1">
          <div class="x_body_top">
            <div class="x_body_img">
              <img src="/logo.png" alt="logo" />
            </div>
            <div class="x_body_text" @click="setMode('otp_verification')">
              Boldseams Couture
            </div>
          </div>
        </section>
        <section class="_main_content_2">
          <div class="_section_card">
            <div class="_card_header">
              <div class="_card_head_l">My Profile</div>
              <div class="_card_head_r">
                <a
                  href="javascript:void(0)"
                  class="_under_ine"
                  @click="setMode('change_password')"
                  >Change Password
                </a>
                <a
                  href="javascript:void(0)"
                  class="_under_ine"
                  @click="setMode('edit_profile')"
                  >Edit
                </a>
              </div>
            </div>
            <div class="_card_form">
              <div class="_card_form_item">
                <label class="label"> Name </label>
                <input type="text" class="_form_input" />
              </div>
              <div class="_card_form_item">
                <label class="label"> Email </label>
                <input type="text" class="_form_input" />
              </div>
              <div class="_card_form_item">
                <label class="label"> Phone Number </label>
                <input type="text" class="_form_input" />
              </div>
            </div>
          </div>
        </section>
        <section class="_main_content_3">
          <div class="_section_card">
            <div class="_card_header">
              <div class="_card_head_l">My Profile</div>
              <div class="_card_head_r">
                <a href="javascript:void(0)" @click="setMode('business_add')">
                  <svg
                    width="20px"
                    height="20px"
                    role="img"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 512 512"
                    class="svg-inline--fa fa-plus-circle fa-w-16 fa-2x"
                  >
                    <path
                      fill="currentColor"
                      d="M256 8C119 8 8 119 8 256s111 248 248 248 248-111 248-248S393 8 256 8zm144 276c0 6.6-5.4 12-12 12h-92v92c0 6.6-5.4 12-12 12h-56c-6.6 0-12-5.4-12-12v-92h-92c-6.6 0-12-5.4-12-12v-56c0-6.6 5.4-12 12-12h92v-92c0-6.6 5.4-12 12-12h56c6.6 0 12 5.4 12 12v92h92c6.6 0 12 5.4 12 12v56z"
                      class=""
                    ></path>
                  </svg>
                </a>
                <a href="javascript:void(0)" @click="setMode('business_add')"
                  >Add Business
                </a>
              </div>
            </div>
            <div class="_card_form">
              <div class="_card_form_item">
                <div class="_form_div">
                  <div class="_form_top">
                    <a
                      href="javascript:void(0)"
                      @click="setMode('business_detail')"
                      >Boldseams Stitches</a
                    >
                  </div>
                  <div class="_form_bottom">RC-907864</div>
                </div>
              </div>
              <div class="_card_form_item">
                <div class="_form_div">
                  <div class="_form_top">
                    <a
                      href="javascript:void(0)"
                      @click="setMode('congratulation')"
                      >Show Congratulation Tab</a
                    >
                  </div>
                  <div class="_form_bottom">RC-905374</div>
                </div>
              </div>
              <div class="_card_form_item">
                <div class="_form_div">
                  <div class="_form_top">
                    <a
                      href="javascript:void(0)"
                      @click="setMode('otp_verification')"
                      >Show OTP Tap</a
                    >
                  </div>
                  <div class="_form_bottom">RC-907864</div>
                </div>
              </div>

              <div class="_card_form_item">
                <div class="_form_div">
                  <div class="_form_top">
                    <a href="javascript:void(0)">Wigan Automobile </a>
                  </div>
                  <div class="_form_bottom">524374</div>
                </div>
              </div>
            </div>
          </div>
        </section>
      </div>
    </div>

    <div
      class="modal fade"
      id="exampleModal"
      tabindex="-1"
      aria-labelledby="exampleModalLabel"
      aria-hidden="true"
    >
      <div class="modal-dialog modal-lg">
        <div class="modal-content">
          <div class="x_modal">
            <div class="x_modal_head">
              <div class="x_modal_head_left">
                <span v-if="current_modal == 'edit_profile'">
                  Edit Profile Details
                </span>
                <span v-if="current_modal == 'change_password'"
                  >Change Password
                </span>
                <span v-if="current_modal == 'business_detail'">
                  Business Details -
                  <span class="sub_head">Boldseams Couture</span>
                </span>
                <span v-if="current_modal == 'business_add'">
                  Add Business
                </span>
                <span v-if="current_modal == 'otp_verification'">
                  OTP Verification
                </span>
                <span v-if="current_modal == 'congratulation'"> Success </span>
              </div>
              <div class="x_modal_head_right">
                <div class="modal_svg">
                  <svg
                    data-dismiss="modal"
                    width="20px"
                    height="20px"
                    role="img"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 320 512"
                    class="svg-inline--fa fa-times fa-w-10 fa-2x"
                  >
                    <path
                      fill="currentColor"
                      d="M193.94 256L296.5 153.44l21.15-21.15c3.12-3.12 3.12-8.19 0-11.31l-22.63-22.63c-3.12-3.12-8.19-3.12-11.31 0L160 222.06 36.29 98.34c-3.12-3.12-8.19-3.12-11.31 0L2.34 120.97c-3.12 3.12-3.12 8.19 0 11.31L126.06 256 2.34 379.71c-3.12 3.12-3.12 8.19 0 11.31l22.63 22.63c3.12 3.12 8.19 3.12 11.31 0L160 289.94 262.56 392.5l21.15 21.15c3.12 3.12 8.19 3.12 11.31 0l22.63-22.63c3.12-3.12 3.12-8.19 0-11.31L193.94 256z"
                      class=""
                    ></path>
                  </svg>
                </div>
              </div>
            </div>
            <div class="x_modal_body">
              <div class="x_modal_form" v-if="current_modal == 'edit_profile'">
                <div class="x_modal_form_item">
                  <label for="" class="">First Name</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item">
                  <label for="" class="">Last Name</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item">
                  <label for="" class="">Email</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item">
                  <label for="" class="">Phone Number</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_form_button">
                  <button type="button" class="x_button">Save</button>
                </div>
              </div>

              <div
                class="x_modal_form"
                v-if="current_modal == 'change_password'"
              >
                <div class="x_modal_form_item">
                  <input
                    type="text"
                    class="x_modal_input"
                    placeholder="Old Password"
                  />
                </div>
                <div class="x_modal_form_item">
                  <input
                    type="text"
                    class="x_modal_input"
                    placeholder="New Password"
                  />
                </div>
                <div class="x_modal_form_item">
                  <input
                    type="text"
                    class="x_modal_input"
                    placeholder="Confirm Password"
                  />
                </div>
                <div class="x_form_button">
                  <button type="button" class="x_button">Save</button>
                </div>
              </div>

              <div
                class="x_modal_form"
                v-if="current_modal == 'otp_verification'"
              >
                <div class="x_otp_text">
                  An OTP Code was sent to your phone and email, kindly input the
                  code below
                </div>
                <div class="x_otp_wrap">
                  <div class="x_otp_item">
                    <input type="text" class="otp_input" />
                  </div>
                  <div class="x_otp_item">
                    <input type="text" class="otp_input" />
                  </div>
                  <div class="x_otp_item">
                    <input type="text" class="otp_input" />
                  </div>
                  <div class="x_otp_item">
                    <input type="text" class="otp_input" />
                  </div>
                </div>
                <div class="x_form_button">
                  <button type="button" class="x_button">Submit</button>
                </div>
              </div>

              <div
                class="x_modal_form"
                v-if="
                  current_modal == 'business_detail' ||
                  current_modal == 'business_add'
                "
              >
                <div class="x_modal_img_wrap">
                  <div class="x_modal_img">
                    <img src="/logo.png" alt="logo" />
                  </div>
                  <div class="x_modal_text">Boldseams Couture</div>
                </div>
                <div class="x_modal_form_item">
                  <label for="" class="">Business Name</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Phone Number</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Business Type</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Email</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Industry</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Country</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Rc Number</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">State</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item input_half">
                  <label for="" class="">Local council</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div class="x_modal_form_item">
                  <label for="" class="">Business Address</label>
                  <input type="text" class="x_modal_input" />
                </div>
                <div
                  class="x_form_button"
                  v-if="current_modal == 'business_add'"
                >
                  <button type="button" class="x_button">Edit</button>
                </div>
                <div class="x_form_button" v-else>
                  <button type="button" class="x_button">Save</button>
                </div>
              </div>
              <div
                class="x_modal_form"
                v-if="current_modal == 'congratulation'"
              >
                <div class="x_congratulation_wrap">
                  <div class="x_congs_img">
                    <img src="/clap_2.png" />
                  </div>
                  <div class="x_congs_text">Congratulations</div>
                  <div class="x_congs_text_s">
                    Your Password has been changed successfully
                  </div>

                  <div class="x_form_button">
                    <button type="button" class="x_button">Save</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import SideBar from './components/SideBar.vue'
export default {
  name: "App",
  data() {
    return {
      current_modal: "",
    };
  },
  components: {
    // SideBar
  },
  methods: {
    setMode(current_modal) {
      this.current_modal = current_modal;
      this.$refs.xnxnxnx.click();
    },
  },
};
</script>
<style>
.sub_head {
  font-weight: 600;
}
.x_otp_wrap {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}

.x_otp_item {
  width: 50px;
  height: 50px;
  margin: 10px;
  background: #fafafa;
  box-shadow: 0 0 3px 0 #f4f4f4;
}
.otp_input {
  width: 100%;
  height: 100%;
  border: 1px solid #f4f4f4;
  background: #fafafa;
  display: flex;
  align-items: center;
  justify-content: center;
}
.otp_input:focus {
  outline: none;
  border: 1px solid black;
}
.x_otp_text {
  padding: 20px 22%;
  text-align: center;
  font-size: 14px;
  font-weight: 600;
  color: black;
  margin-top: 20px;
}
.x_modal_head_right {
  display: flex;
  justify-content: right;
}
.modal_svg {
  /* border:1px solid red; */
  width: 23px;
  height: 23px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}
@media (min-width: 992px) {
  .modal-lg,
  .modal-xl {
    max-width: 600px !important;
  }
}
.x_modal {
  width: 100%;
  margin: auto;
  min-height: 300px;
}
.modal-content {
  border-radius: 5px !important;
  border: none;
  overflow: hidden !important;
}
.x_button {
  border: none !important;
  background: #0995c8;
  color: white;
  padding: 5px 49px;
  border-radius: 5px;
}
.x_button:focus {
  outline: none !important;
  border: 1px solid #ccc;
}
.x_form_button {
  width: 100%;
  display: flex;
  justify-content: center;
  margin-top: 50px;
}
.x_modal_form {
  width: 100%;
  padding: 5px 5px 10px 5px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
.x_modal_img_wrap {
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  margin-bottom: 15px;
}
.x_modal_img {
  width: 70px;
  height: 70px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.x_modal_img img {
  width: 100%;
}
.x_modal_text {
  font-weight: 500;
  font-size: 20px;
  color: #0979a2;
}
.x_modal_form_item {
  width: 100%;
  display: flex;
  padding: 5px;
  flex-direction: row;
  position: relative;
  margin-top: 20px;
}
.x_congratulation_wrap {
  display: flex;
  width: 100%;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.x_congs_text {
  font-weight: 600;
  margin-top: 30px;
}
.x_congs_text_s {
  font-weight: 600;
  color: #333333;
  margin-top: 10px;
  font-size: 12px;
}

.input_half {
  width: 50%;
}
.x_modal_input {
  border: 2px solid #e9e9e9;
  border-radius: 5px;
  width: 100%;
  padding-left: 10px;
  font-size: 15px;
  height: 35px;
  top: 0;
}
.x_modal_input:focus {
  outline: none !important;
  border: 2px solid #0995c8;
}
.x_modal_form_item label {
  position: absolute;
  top: -5px;
  left: 15px;
  font-size: 13px;
  font-weight: 400;
  color: #a3a3a3;
  background: white;
}
.x_modal_head {
  height: 40px;
  width: 100%;
  justify-content: space-between;
  box-shadow: 0 0px 15px 0 #097da7 inset;
  display: flex;
  align-items: center;
  background: #0995c8;
  padding: 0 10px;
  color: white;
}
._body_container {
  width: 100%;
  min-height: 100vh;
  background: #fafafa;
  display: flex;
  justify-content: flex-start;
  flex-direction: column;
  color: rgb(156, 156, 156);
}
._head_container {
  min-height: 50px;
  width: 100%;
  padding: 5px 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
._head_left {
  display: flex;
  flex-direction: row;
  align-items: center;
}
._head_left_logo {
  font-size: 22px;
  font-weight: 700;
  padding: 4px 7px;
  margin: 5px 10px 5px 0;
  border-radius: 10px;
  border: 1px solid #eeeeee;
}
._head_left_text {
  font-weight: 700;
  color: #333333;
  font-size: 16px;
}
._head_right {
  display: flex;
  flex-direction: row;
}
._head_right_text {
  display: flex;
  flex-direction: column;
  font-size: 15px;
  justify-content: flex-end;
}
._head_right_text {
  text-align: right;
  font-size: 14px;
  min-width: 150px;
}
._head_right_text a {
  font-size: 12px;
  text-decoration: underline;
  font-weight: 500;
}
._head_right_logo {
  position: relative;
}
._head_count {
  position: absolute;
  top: 0px;
  right: -1px;
  background: red;
  width: 15px;
  height: 15px;
  font-size: 10px;
  font-weight: 700;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
}
._body_container {
  min-height: calc(100vh - 50px);
  display: flex;
  width: 100%;
  flex-direction: row;
  justify-content: flex-start;
}
._main_bread_crom {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}
.icon_wrap {
  margin: 10px;
}
.icon_wrap svg {
  stroke-width: 6;
  color: black;
}
._bread_left {
  font-size: 15px;
  font-weight: 500;
  height: 38px;
  display: flex;
  flex-direction: row;
}

._bread_first {
  border: 2px solid #eeeeee;
  border-right: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 400;
  background: #eeeeee;
}
._bread_item {
  min-width: 150px;
  padding-right: 20px;
  padding-left: 20px;
  height: 100%;
  background-color: white;
  display: flex;
  align-items: center !important;
  justify-content: center;
}
._bread_item_2 {
  min-width: 150px;
  padding-right: 15px;
  padding-left: 20px;
  height: 100%;
  background-color: #eeeeee;
  align-items: center;
  display: flex;
  color: #7c7c7c;
  justify-content: center;
}
._bread_second {
  /* border: 1px solid #eeeeee; */
  border-right: 0;
  height: 100%;
  display: flex;
  position: relative;
  align-items: center;
  justify-content: center;
  word-wrap: wrap none;
}
._bread_first:after {
  content: "";
  width: 0;
  height: 0;
  right: 0;
  border-top: 18px solid transparent;
  border-left: 15px solid white;
  border-bottom: 18px solid transparent;
}

._bread_second:after {
  content: " ";
  width: 20px;
  height: 38px;
  right: 0;
  background: #eeeeee;
  border: 1px solid #eeeeee;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}
.main_bread_crom {
  height: 30px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  border: 1px solid red;
}
._side_bar {
  width: 250px;
  min-height: calc(100vh - 50px);
  background: #0995c8;
}

._main_content {
  display: flex;
  flex-grow: 1;
  flex-direction: column;
}
._section_card {
  border-radius: 5px;
  border: 1px solid #ccc;
  padding: 20px 40px;
  background: white;
}
.x_body_top {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.x_body_img {
  width: 100px;
  height: 100px;
  display: flex;
  align-items: center;
}

.x_body_text {
  font-weight: 500;
  font-size: 20px;
  color: #0979a2;
}
._main_content section {
  width: 100%;
  min-height: 150px;
  padding: 20px;
}
._card_header {
  width: 100%;
  display: flex;
  margin-bottom: 10px;
  flex-direction: row;
  justify-content: space-between;
}
._card_head_l {
  font-weight: 700;
  margin: 0 10px;
}
._card_header a._under_ine {
  margin: auto 5px;
  text-decoration-line: underline;
}
._card_header a {
  margin: auto 5px;
}
._card_form {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-start;
  max-width: 980;
}
._card_form_item {
  width: 50%;
  flex-basis: 1;
  min-width: 300px;
  display: flex;
  border: none;
  flex-direction: column;
  padding: 0 10px;
}
._form_input {
  border: none;
  border-bottom: 1px solid #ccc;
  outline: none;
  height: 25px;
}
._form_input:active {
  outline: none !important;
  border: none;
  border-bottom: 1px solid red;
}
label {
  margin: 0;
}

._form_div {
  border: 1px solid #ccc;
  margin: 10px auto;
  width: 100%;
  flex-basis: 1;
  border-radius: 2px;
  display: flex;
  flex-direction: column;
  padding: 5px 20px;
  height: 70px;
}
._form_top {
  margin-bottom: 5px;
}
._form_top a {
  text-decoration: none;
  font-weight: 600;
}
@media (max-width: 600px) {
  ._side_bar {
    display: none;
  }
  ._card_form {
    justify-content: center;
  }
  ._card_form_item {
    padding: 0 2px;
  }
}
</style>