<style>
  .section-title {
    text-align: center;
    padding-bottom: 30px;
  }
  h2 {
    color: #dc143c;
    text-transform: uppercase;
    font-size: 32px;
    font-weight: 600;
    margin-bottom: 20px;
    padding-bottom: 20px;
    position: relative;
    font-family: "Poppins", sans-serif;
  }
  .info-box h3 {
    font-size: 20px;
    color: #777;
    font-weight: 700;
    margin: 10px 0;
    color: #dc143c;
    text-transform: uppercase;
    margin-bottom: 20px;
    padding-bottom: 20px;
    position: relative;
    font-family: "Raleway", sans-serif;
  }
</style>

<section id="contact" class="contact section-bg">
  <div class="container">
    <div class="section-title">
      <h2 data-aos="fade-in" class="aos-init aos-animate">Contact</h2>
      <p data-aos="fade-in" class="aos-init aos-animate">
        You can reach out to us with one of the options below
      </p>
    </div>

    <div class="row">
      <div class="col-lg-6">
        <div class="row">
          <div class="col-md-12">
            <div class="info-box aos-init aos-animate" data-aos="fade-up">
              <i class="bx bx-map" />
              <h3>Our Address</h3>
              <p>Abuja Office: Novare Central (shoprite) Wuse Zone 5, Abuja.</p>
              <p>Vienna Office: Franz-Asenbauergasse 12-16/5/6, 1230 Vienna.</p>
            </div>
          </div>
          <div class="col-md-6">
            <div
              class="info-box mt-4 aos-init aos-animate"
              data-aos="fade-up"
              data-aos-delay="100">
              <i class="bx bx-envelope" />
              <h3>Email Us</h3>
              <p>Info@codedsnippet.online</p>
            </div>
          </div>
          <div class="col-md-6">
            <div
              class="info-box mt-4 aos-init aos-animate"
              data-aos="fade-up"
              data-aos-delay="100">
              <i class="bx bx-phone-call" />
              <h3>Call Us</h3>
              <p>07060962656 &amp; +43 676 7212185</p>
            </div>
          </div>
        </div>
      </div>

      <div class="col-lg-6">
        <form
          action="forms/contact.php"
          method="post"
          role="form"
          class="php-email-form aos-init aos-animate"
          data-aos="fade-up">
          <div class="form-row">
            <div class="col-md-6 form-group">
              <input
                type="text"
                name="name"
                class="form-control"
                id="name"
                placeholder="Your Name"
                data-rule="minlen:4"
                data-msg="Please enter at least 4 chars" />
              <div class="validate" />
            </div>
            <div class="col-md-6 form-group">
              <input
                type="email"
                class="form-control"
                name="email"
                id="email"
                placeholder="Your Email"
                data-rule="email"
                data-msg="Please enter a valid email" />
              <div class="validate" />
            </div>
          </div>
          <div class="form-group">
            <input
              type="text"
              class="form-control"
              name="subject"
              id="subject"
              placeholder="Subject"
              data-rule="minlen:4"
              data-msg="Please enter at least 8 chars of subject" />
            <div class="validate" />
          </div>
          <div class="form-group">
            <textarea
              class="form-control"
              name="message"
              rows="5"
              data-rule="required"
              data-msg="Please write something for us"
              placeholder="Message" />
            <div class="validate" />
          </div>

          <div class="text-center">
            <button type="submit " class="btn btn-red">Send Message</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</section>
