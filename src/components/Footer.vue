<template>
  <div class="contact-one">
    <img
      src="data:image/png;base64,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"
      class="contact-one__bg-shape-1"
      alt=""
    />
    <div class="container">
      <div class="row">
        <div class="col-lg-7">
          <form class="contact-form-validated contact-one__form">
            <div class="block-title text-left">
              <p>Contact Now</p>
              <h3>Have Question? Write a Message</h3>
            </div>
            <div class="row">
              <div class="col-lg-6">
                <input type="text" placeholder="Name" name="name" />
              </div>
              <div class="col-lg-6">
                <input type="text" placeholder="Email Address" name="email" />
              </div>
              <div class="col-lg-6">
                <input type="text" placeholder="Subject" name="subject" />
              </div>
              <div class="col-lg-6">
                <input type="text" placeholder="Phone Number" name="phone" />
              </div>
              <div class="col-lg-12">
                <textarea placeholder="Write Message" name="message"></textarea>
              </div>
              <div class="col-lg-12 text-left">
                <button type="submit" class="thm-btn contact-one__btn">
                  <span>Send Message</span>
                </button>
              </div>
            </div>
          </form>
          <div class="result"></div>
        </div>
        <div class="col-lg-5 d-flex wow fadeInRight" data-wow-duration="1500ms">
          <div class="my-auto">
            <div class="contact-one__image">
              <img
                src="/_next/static/images/contact-1-1-12b719fbe7c3858a340cf121f6d5b947.jpg"
                alt=""
              />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="cta-three">
      <img
        src="/_next/static/images/cta-three-bg-1-1-d5f9cdbf639e05d3468fad400e9fd152.png"
        class="cta-three__bg-1"
        alt=""
      /><img
        src="/_next/static/images/cta-three-bg-1-2-fca9cc9abb003671e69d94630e769704.png"
        class="cta-three__bg-2"
        alt=""
      />
      <div class="text-center container">
        <h3>
          Download our App Today &amp; <br />
          Experience Endless Possibilities
        </h3>
        <p>and get started with a free 1 month trial for your business</p>
        <div class="cta-three__btn-wrap">
          <a href="#" class="cta-three__btn"
            ><i class="fa fa-play"></i><span>Get in</span><b>Google Play</b></a
          ><a href="#" class="cta-three__btn"
            ><i class="fab fa-apple"></i><span>Get in</span
            ><b>Apple Store</b></a
          >
        </div>
      </div>
    </div>
    <div>
      <section class="mailchimp-one">
        <div class="container wow fadeInUp">
          <div class="inner-container">
            <div class="mailchimp-one__icon">
              <i class="apton-icon-mail"></i>
            </div>
            <form action="#" class="mailchimp-one__form">
              <input
                type="text"
                placeholder="Enter your email address"
                name="email"
              /><button class="thm-btn mailchimp-one__btn" type="submit">
                <span>Register Now</span>
              </button>
            </form>
          </div>
        </div>
      </section>
      <footer class="site-footer">
        <div class="site-footer__upper">
          <div class="container">
            <div class="row">
              <div class="col-lg-4">
                <div class="footer-widget footer-widget__about">
                  <a href="index.html"
                    ><img
                      src="/_next/static/images/logo-1-1-57382e3eb673ea7f40dec59e4e6f577b.png"
                      width="129"
                      alt=""
                  /></a>
                  <p>
                    Lorem Ipsum is simply dummy text the <br />
                    printing and setting industry. Lorm Ipsum<br />
                    has been the text ever.
                  </p>
                </div>
              </div>
              <div class="col-lg-5">
                <div class="footer-widget__links-wrap">
                  <div class="footer-widget">
                    <h3 class="footer-widget__title">Company</h3>
                    <ul class="list-unstyled footer-widget__links-list">
                      <li><a href="#">About</a></li>
                      <li><a href="#">Our Team</a></li>
                      <li><a href="#">Contact</a></li>
                      <li><a href="#">Services</a></li>
                    </ul>
                  </div>
                  <div class="footer-widget">
                    <h3 class="footer-widget__title">Explore</h3>
                    <ul class="list-unstyled footer-widget__links-list">
                      <li><a href="#">News</a></li>
                      <li><a href="#">Features</a></li>
                      <li><a href="#">Download</a></li>
                      <li><a href="#">Free Trial</a></li>
                    </ul>
                  </div>
                  <div class="footer-widget">
                    <h3 class="footer-widget__title">Links</h3>
                    <ul class="list-unstyled footer-widget__links-list">
                      <li><a href="#">Help</a></li>
                      <li><a href="#">Privacy Policy</a></li>
                      <li><a href="#">Terms of Use</a></li>
                      <li><a href="#">Services</a></li>
                    </ul>
                  </div>
                </div>
              </div>
              <div
                class="
                  col-lg-3
                  d-flex
                  align-items-center
                  justify-content-xl-end
                  justify-content-lg-end
                  justify-content-md-center
                  justify-content-sm-center
                "
              >
                <div class="footer-widget">
                  <div class="footer-widget__social">
                    <a href="#"><i class="fab fa-facebook-square"></i></a
                    ><a href="#"><i class="fab fa-twitter"></i></a
                    ><a href="#"><i class="fab fa-instagram"></i></a
                    ><a href="#"><i class="fab fa-pinterest-p"></i></a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="site-footer__bottom">
          <div class="container text-center">
            <p>© copyright 2020 by Layerdrops.com</p>
          </div>
        </div>
      </footer>
    </div>
    <a class="scroll-to-top"><i class="fa fa-angle-up"></i></a>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

