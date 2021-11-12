<template>
  <section class="team-one" id="team">
    <img
      src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASQAAAKhCAMAAADOsiMoAAAAn1BMVEUAAAD29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vv29vt8b2JxAAAANHRSTlMAA/z4Bu4P9Csk6gvl01JMxLEf27idkBQciTHPbVs7cWdBNr+WfKZG4NfJd2Cighj6vKpWEWYtYQAADJNJREFUeNrs2oteokAUx/EjhEgJaIiblZfybrhW/t//2bbdbmuKg6VwhjnfR/h9GDgzA9W81QWJ/fDCcmZ+oxl3HpKgdynJtmGLMx8uO4OwViXxBumcxWS8vpYniwhKs6fR7fSyQgZDRu5NfHtn6grEQWbN8dTAUjhcNOn3zsgk+B670Ql/kSnwA/5obUYo/JDfDsr/ksLPWY1xr9wTAo7DeU5WVFo4GmsxvqZywlHNRtMyLjwcmxOHpRuicALusmSdcBpOXKZ1h5Opt++pJHBK0fiSygCnZQ2TEpza4eTcUY80hzz4fb03wsiHvdT5cUJubgbaHhcgR27bIy0hX61QxxkTeZsP9JsJkD+nc0V6QREelzXSCQrS1GkkQGEWIekCBboJSA8olL/WYiJAweZdDTKhcFHCPhMYiLg/TWDB5/2lAxMNznMT2Gjxvf8FIxOuJyngxBrxPOYFL06f490vuIkY7lXAz5DdGxwMWTGzH8LAkvvA6tUEpuZT4gNsPfP52QJ88Vlz4MxnsqEDbzGLERzMnXepeGCvWfxVJvhzB3QYEyMBQ48OYWYkuP0KZWdoJGBRo8yMjQR7XKGMzI0ELDzKxuRIcG8pE6MjAU9XlIHhkeAEpGZ6JCCukopEQnRPChIJeHyg/STSX60V7SOR/qlPaQ+J9Mr6XaFUEundcEVpJNKH+h2lkEifrD7tJpH+N7mgXSTSBt+jHSTSJiekbRLpqx2zgETa0qrSFxJpW1SjTRJpB2dKGyRSholJIu0Wn9EniZTiqUofJFKauUfvJFKq8x69kUjp7DW9kkgZPnISaa92hV5IpP2ez4hIIikMq0QS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"
      class="team-one__bg-shape-1"
      alt=""
    /><img
      src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAKEAAAC2CAMAAACGXB2nAAACkVBMVEUAAADwYUDNXmWfWZfBXXLbX1bwYUD8YzLwYj/xYj7xYj+7XHiLV63jYE25XHvKXmnwYj/gYFC2XH6CVrbwYkDfYFL7YzP8YzP8YzK4XHynWo78YzPOXmTiYE78YzK5XHviYE/8YzK4XHt7Vr79YzHwYT/PXmOkWpLeYFOLV6zQXmKkWpLNXmXxYj93VcLfYFPMXmZaUuLgYFCBVrefWZi5XHv7YzPPXmONWKrPXmOjWpKPWKilWpDMXmfiYE7yYj2NV6vgYFHwYj/yYj3wYj92VcPxYj79YzHgYFHwYj/hYE+HV7LjYE3vYUHQXmL7YzPgYFH8YzNlU9XiYE55VcChWZW4XHuNV6vPXmSiWZN1VcR5VcF7Vb+iWZRbUuGnWo90VcV0VcWQWKe7XHn8YzP9YzGQWKfQXmLeYFPxYj5SUellU9aiWpOhWZb8YzOjWpO1XH+8XHfiYE62XH68XHjOXmS8XHijWpPgYFBSUeqNV6rLXmdVUuaJV6/hYE/jYE25XHthU9piU9m2XH1lU9Z3VcGhWpSNWKtnU9OgWZZRUevNXmVHUPZGUPagWZbvYkBkU9ZnU9OQWKf7YzT9YzFUUufhYE9lU9V5VcCQWKekWpHhYE9kU9aQWKfeYFP7YzNjU9h0VcX7YzRGUPdUUudlU9aiWpPeYFO1XH+8XHf8YzJHUPVkU9a1XH+8XHdlU9XMXmaPWKhnU9P9YzFGUPd0VcV3VcJjU9d6Vb/9YzHwYkDPXmPiYE6lWpHgYFD7YzOOV6rxYj7MXma4XHy5XHqhWpXfYFKiWpN2VcO2XH27XHnLXmdjU9eMV6z7YzRHUPbQXmJmU9V4VcB6Vb+KV63yYj1TUehVUuZiU9neYFOQWKdCW6z2AAAAuXRSTlMAgDAQEBBggBAw77+AgEBAQM+/ICDv79+/gEAwIGBAUCAgr4BgUEAwMO/vz8/Pv6+fQEAwICAQv4+AYFDv7+/fv7+/v6+fn5+Pj4BwcHBgYFBQMDDv79Ovr4+AYEBAICAQ7+/v7+/f39/fv7+/r6+fn5+fj4+PgHBwYGBgUEBAQDAQ7+/f39/Pv7+vcDDv39/Pz8/Pz7+/r6+vr6+fn5+fj4+PiICAgIBwcHBgYGBgUFBAEBDf34BwUGch56cAAAXnSURBVHja7Z3lWxRRFMYPG7QrocKKiAlioLgqIHYrJnZhd3d3d3d3d+4SoqCsimLXX+O9fvAx9pxFh5k9C/P7+n55H9j7zG/u3AAvoNZYe0QUcMZutz+KAM7Ihq+BM/wbRoqGfsCaWn5VQadkCakArAmY5HB0Bc60f+xwOGoDYz7Khj7AmNayoS8wprZo2MAfOFPBh/VfkCfVqzaj4r6NwcP42e2V+uDx7KycinVAA2i3qYSm0VlZOc8agkeh7aucbPgVPAr9N+wuG7YFj9JZNOyFpuZQz/8OIapqdSpe3rga6Pwb/iEBVFwl1gCeJSDQ4WiHxz0zM580Ao/SgHabuqLhSwN4EtoPDW9kw/LwT5S5v6H8HXZg/TvkP5Y5ouiZYrJYTOACNs/lpmPy89Y0RUIN3SYUjWe9yM97PtNlxMQPg2TDMFcJF8eeKxvOcZ3xeE8xDcjPG+B6qLB517NYQOcf5xxiU25S8XAjlmg1b5NCP5dnZK9PRSKt5r7ekG4Tl51d8HSTy4iJH1aWDZ82QVIV5mAxP6yCpSNkw/6Aock8dmzdzCdL8Lh5dkH/4UCgxbeAWBOVGodDWYT+JmVe2K0OETe1WhH50uq7nvTDZ73ReKX0w5VonJpsVNW+lPvh7tz4NE38sOL/+uG33NxXG2wqfqN374fzZUMrGh8SDT+kqrzOoUtWTqgZ98Og/LwwExobN+S+SgYdfoT49PAn4p4pW0x4alxwvjmojK8wh0C84jxhDvUBpZ4wh8FIVqJ+2AONi2NfRixOOxjO3A9rvu93HxTTQTYMQeMJ7v1wO2AMe//Ouc4GCvFv7wj0wWPDhMyWlB+2KFgfh8c1+zkTRoKO9ty57NeLiKt169abiC1Wq4WIU4ODlQ/fvcIcTuMFWwlziMYLSnPAKy4W5hAfroF9TUTjGrJhDTQeL90mmLMfjqYbbsyA4jBONNyDpitkw+NofEk2vIjGx2TDZWi86+3JVeCePhH2SMIPo1vlNDTj8dz8vDmESAzMjV+Mx+lTCneCjifwbdepAp6aU5LmUX44eOoCwLF1TBgKSvGRfohXHOTeD6ehaXi/d07nEFBIIOmHZmV++F40HKWuH1ZR5ocl0rCTbBiAxvVFw5YmLDW2EA3rkX7o7IjGGYnF88NOjh2+hB8OyqxvwOO4egXTmuDx0HXOjoQfnj0LOupQvXOkXzM87nuk7ULAiQkKiyHitDYDbXh6+9yUo8WQhwhhDtNpP7yAF5TmgFcMpv3wwNvCwrWrOPvhW9HwS6IKDRX4IdGQ9sNI2g+7oPF12fAaGifLhjbcYEXD1e7/y1HTI08QI6X3/rZdAGd+UJiViJPbtEklRsrRKQfSQUddtrrUr3YdQgg/bJQ0iHrqHZ46w4jHwxISKPlaum/yIviFK9uKtv3dsas0B9wPk9ybwybcD6U5nMILfv786dMvFTOKBHdd+CFlX2Y17WuzbDgZfpJYJEEaKvJDYwk13Fok4fxfhs2i4BmNR8rB30dK+rkb1EiBK2cSwaPcEM+Uk8CZtfK5nMH5qcfFHJa5ach6dk66DWuDTV9buPoq67cA0ZH5m5SOutCzIrXx2JCkeFaE88yS7cfMEvvZOSfnGc4fDe+V/lliOdMeQPjhFo/PtOv8CfuvZg+Yf3ncmcj86+3VEvu+HKrID9NK/yoC/isxdP6i9K+qUntl2pCRDPwwDrevhHBQTGvlfggYQx+WjVWm/Ffq6nhi1X0Nd6vu2e9cWMZ5d7DY/REfzHwHzcBw3ruQbt3SZidXY3c7uXS8bUch/12Z/He28t8drHiHdX9cbnjsUh9sxFNtdvob6J3+I6BMwv7ECf6ndvA/+cTbT4+hThd074dMTjEaoLp+RdWiT4KKJk+CiokxgY63nUjG/1Q3/ifj6acLloVTLvmPZY6wP7GW/6m/Ck4XpODihyhsHJuAyXsKBZd3PR1vvNGA/60Q/G/W4H87Cf8bXvjfksP/piGOsL/xiv+tYfxvXvOOhrxvAOR/iyJ3vgMJXIf0o2BuowAAAABJRU5ErkJggg=="
      class="team-one__bg-shape-2"
      alt=""
    />
    <div class="container">
      <div class="block-title text-center">
        <p>Expert People</p>
        <h3>Meet Our Professional Team Members</h3>
      </div>
      <div class="row">
        <div class="col-lg-3 col-md-6 col-sm-12">
          <div class="team-one__single">
            <div class="team-one__circle"></div>
            <div class="team-one__inner">
              <h3>Nathaniel McKenzie</h3>
              <p>App Designer</p>
              <div class="team-one__image">
                <img
                  src="/_next/static/images/team-1-1-c4ea3e70dbf18776dc400ecee89de41d.jpg"
                  alt=""
                />
              </div>
              <div class="team-one__social">
                <a href="#"><i class="fab fa-facebook-square"></i></a
                ><a href="#"><i class="fab fa-twitter"></i></a
                ><a href="#"><i class="fab fa-instagram"></i></a>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6 col-sm-12">
          <div class="team-one__single">
            <div class="team-one__circle"></div>
            <div class="team-one__inner">
              <h3>Ronald Parks</h3>
              <p>App Designer</p>
              <div class="team-one__image">
                <img
                  src="/_next/static/images/team-1-2-30c2d6ff50fdca9b3739920b9c2cec2b.jpg"
                  alt=""
                />
              </div>
              <div class="team-one__social">
                <a href="#"><i class="fab fa-facebook-square"></i></a
                ><a href="#"><i class="fab fa-twitter"></i></a
                ><a href="#"><i class="fab fa-instagram"></i></a>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6 col-sm-12">
          <div class="team-one__single">
            <div class="team-one__circle"></div>
            <div class="team-one__inner">
              <h3>Rachel Walker</h3>
              <p>App Designer</p>
              <div class="team-one__image">
                <img
                  src="/_next/static/images/team-1-3-8476d5b7ff6158d4b109ecf1a7708b59.jpg"
                  alt=""
                />
              </div>
              <div class="team-one__social">
                <a href="#"><i class="fab fa-facebook-square"></i></a
                ><a href="#"><i class="fab fa-twitter"></i></a
                ><a href="#"><i class="fab fa-instagram"></i></a>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6 col-sm-12">
          <div class="team-one__single">
            <div class="team-one__circle"></div>
            <div class="team-one__inner">
              <h3>Willie Castillo</h3>
              <p>App Designer</p>
              <div class="team-one__image">
                <img
                  src="/_next/static/images/team-1-4-5db54e10654ae21ebda2ed62c98dfde1.jpg"
                  alt=""
                />
              </div>
              <div class="team-one__social">
                <a href="#"><i class="fab fa-facebook-square"></i></a
                ><a href="#"><i class="fab fa-twitter"></i></a
                ><a href="#"><i class="fab fa-instagram"></i></a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="video-one">
      <div
        class="container-fluid"
        style="
          background-image: url(/_next/static/images/video-bg-1-1-3050cfbb09cc9399e29b9434b1957eaa.jpg);
        "
      >
        <div
          class="video-one__content wow fadeInLeft"
          data-wow-duration="1500ms"
        >
          <div class="block-title text-left">
            <p>Video Tutorial</p>
            <h3>Watch Now Our Video Tutorial</h3>
          </div>
        </div>
        <a href="#" class="video-one__btn video-popup"
          ><i class="fa fa-play"></i
        ></a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Team",
  props: {
    msg: String,
  },
};
</script>
