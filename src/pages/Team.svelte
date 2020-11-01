<script>
  export const teams = [
    {
      id: 1,
      name: "Gabriel Aloho",
      title: "CTO",
      picture: "images/aloho.jpg",
      about:
        "Gabriel is a trained Android Developer with the Andela learning community. He has been into ICT for over a decade now. He is the founder of Code Snippet and the Chief Technology Officer",
    },
    {
      id: 2,
      name: "George Percy Peter",
      title: "Director",
      picture: "images/peter.jpg",
      about:
        "Pastor Peter is a Nigerian-Austrian. He enroled and graduated in our online classes and since then he took interest in our business and invested",
    },
    {
      id: 3,
      name: "Abubakar D Abdulkadir",
      title: "Board Member",
      picture: "images/abubakar.jpg",
      about:
        "Abubakar is a PHD student in University of Saforrd Business School. He invested in the business before it was fully launched and remains one of our best investors.",
    },
    {
      id: 4,
      name: "Aminu Wali",
      picture: "images/aminu.jpg",
      title: "Web Developer",
      about:
        "Aminu is a computer Science student in the University Of Abuja. He has undergone training at Code Snippet and is currently intern.",
    },
  ];
  import { fade, slide } from "svelte/transition";
</script>

<style>
  .row {
    display: flex;
    flex-wrap: wrap;
    margin-right: -15px;
    margin-left: -15px;
  }
  .container {
    transform: skewY(6deg);
  }
  .member {
    text-align: center;
    margin-bottom: 20px;
  }
  .member span {
    font-style: italic;
    display: block;
    font-size: 13px;
  }
  .member h4 {
    font-weight: 700;
    margin: 5px 0;
    font-size: 18px;
    color: #fff;
  }
  .member .social {
    margin-top: 15px;
  }
  section {
    /* background: linear-gradient(180deg, #f2f6fa 0%, #fff 100%); */
    background-color: #dc143ce0;
    transform: skewY(-6deg);
  }
  h1 {
    text-align: center;
    padding: 2rem 0;
    color: #fff;
    text-transform: uppercase;
    font-size: 32px;
    font-weight: 600;
    margin-bottom: 20px;
    padding-bottom: 20px;
    position: relative;
    font-family: "Poppins", sans-serif;
  }
  h1::after {
    content: "";
    display: block;
    border-bottom: 5px solid #ffffff;
    width: 30%;
    margin: 1rem auto;
  }
</style>

<section id="team">
  <div class="container" transition:fade>
    <h1>TEAM</h1>
    <div class="row">
      {#each teams as team}
        <div class="col-xl-3 col-lg-4 col-md-6">
          <div class="member aos-init aos-animate" data-aos="fade-up">
            <div class="pic"><img src={team.picture} alt="Team" /></div>
            <h4>{team.name}</h4>
            <span>{team.title}</span>
            <div class="social">
              <a href=""><i class="icofont-twitter" /></a>
              <a href=""><i class="icofont-facebook" /></a>
              <a href=""><i class="icofont-instagram" /></a>
              <a href=""><i class="icofont-linkedin" /></a>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
