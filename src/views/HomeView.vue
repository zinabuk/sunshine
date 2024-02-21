<template>
  <!-- header section -->
  <header
    class="w-full flex justify-between py-6 sticky top-0 z-10 font-semibold bg-white/100 px-4"
  >
    <router-link to="/" class="text-4xl font-bold uppercase"
      >Sunshine</router-link
    >
    <ul class="hidden md:flex">
      <li class="px-4 py-2"><router-link to="/">Home</router-link></li>
      <li class="px-4 py-2"><router-link to="#events">Events</router-link></li>
      <li class="px-4 py-2">
        <router-link to="#about-us">About Us</router-link>
      </li>
      <li class="px-4 py-2">
        <router-link to="#contact-us">Contact Us</router-link>
      </li>

      <li class="px-4 py-2 bg-yellow-500 text-white">
        <button @click="showModal = !showModal">Donate Now</button>
      </li>
    </ul>
    <button class="flex md:hidden" @click="showMenu = !showMenu">
      <img src="@/assets/hamburger.png" alt="" class="w-14 h-12" />
    </button>
  </header>

  <!-- hero section -->
  <section class="w-full relative h-screen flex">
    <img
      src="https://images.pexels.com/photos/1912868/pexels-photo-1912868.jpeg?auto=compress&cs=tinysrgb&w=600"
      alt=""
      class="w-full h-full absolute object-cover object-center inset-0"
    />
    <div class="absolute inset-0">
      <div
        class="h-full w-full bg-gradient-to-r from-black to-transparent flex items-center"
      >
        <div
          class="w-full md:w-1/2 flex flex-col justify-center px-6 md:px-0 text-center md:text-left text-yellow-500 animate-card"
        >
          <h1 class="text-3xl md:text-6xl mb-6">
            Small help together makes a better life
          </h1>
          <button
            class="bg-yellow-500 px-4 py-2 rounded-full text-white self-center md:self-start"
            @click="showModal = !showModal"
          >
            Donate Now
          </button>
        </div>
      </div>
    </div>
  </section>

  <!-- events section -->
  <section
    id="events"
    class="flex w-full justify-center flex-wrap gap-6 py-6 px-4"
  >
    <div class="md:basis-1/4 flex flex-col justify-between shadow-md">
      <img
        src="https://www.savethechildren.org/content/dam/usa/images/donors/zimbabwe-food-crisis-ch1420542-sq.jpg/_jcr_content/renditions/cq5dam.webp_thumbnail.1536.1536.webp"
        alt=""
        class="w-full"
      />
      <h1 class="text-xl text-black font-semibold">Make a donation</h1>
      <p>
        Are you looking to raise money for a cause, project, life event, or
        charity? Donation request letters can be a traditional (yet effective!)
        way to ask companies and individuals for cash and in-kind donations as
        well as sponsorships. You can also use them as invitations to your
        fundraising event.
      </p>
      <a href="" class="text-blue-500">Learn More</a>
    </div>
    <div class="md:basis-1/4 flex flex-col justify-between shadow-md">
      <img
        src="https://www.savethechildren.org/content/dam/usa/images/usp/united-states-nutrition-ch1616179-sq.jpg/_jcr_content/renditions/cq5dam.webp_thumbnail.768.768.webp"
        alt=""
        class="w-full"
      />
      <h1 class="text-xl text-black font-semibold">Fundraising</h1>
      <p>
        A fundraising letter is a great avenue for nonprofits who need to ask
        for donations in a more formal and direct way. Your organization, club,
        or school can use fundraising letters to ask local businesses and
        individuals for cash and in-kind donations. You can even ask for
        sponsorships with fundraising letters.
      </p>
      <a href=""  class="text-blue-500">Learn More</a>
    </div>
    <div class="md:basis-1/4 flex flex-col justify-between shadow-md">
      <img
        src="https://www.savethechildren.org/content/dam/usa/images/usp/united-states-nutrition-ch1616179-sq.jpg/_jcr_content/renditions/cq5dam.webp_thumbnail.768.768.webp"
        alt=""
        class="w-full"
      />
      <h1 class="text-xl text-black font-semibold">Become a volunteer</h1>
      <p>
        Volunteering is a voluntary act of an individual or group freely giving
        time and labor, often for community service. Many volunteers are
        specifically trained in the areas they work, such as medicine,
        education, or emergency rescue. Others serve on an as-needed basis, such
        as in response to a natural disaster.
      </p>
      <a href=""  class="text-blue-500">Learn More</a>
    </div>
  </section>

  <!-- About us section -->
  <section
    id="about-us"
    class="py-6 flex justify-center items-center shadow-sm bg-gray-100"
  >
    <div class="md:w-1/2 flex flex-col items-center">
      <h1 class="text-3xl font-bold text-center text-yellow-600 mb-4">
        About Us
      </h1>
      <hr class="border-2 w-24 border-yellow-400 mb-6" />
      <div class="max-w-2xl text-center">
        <h1 class="text-2xl font-bold mb-4">
          Welcome to Sunshine Childcare NGO!
        </h1>
        <p class="text-lg mb-6">
          At Sunshine Childcare, we believe that every child deserves a
          nurturing and safe environment to grow, learn, and thrive. We are a
          passionate team of dedicated individuals committed to providing
          exceptional care and support to children in need.
        </p>
        <p class="text-lg mb-6">
          Our mission is to ensure the well-being and holistic development of
          children, empowering them to reach their full potential. We strive to
          create a loving and inclusive community where each child is valued,
          respected, and given equal opportunities to flourish.
        </p>
        <p class="text-lg mb-6">
          What sets us apart is our unique approach to childcare. We combine
          professional expertise with a warm and compassionate environment,
          creating a home away from home for the children under our care. Our
          team of experienced caregivers, educators, and volunteers work
          tirelessly to create a safe and stimulating space that promotes
          learning, creativity, and healthy social interactions.
        </p>
        <p class="text-lg mb-6">
          At Sunshine Childcare, we offer a range of services tailored to meet
          the diverse needs of children and families. From early childhood
          education and nutritional support to healthcare initiatives and
          recreational activities, we aim to provide comprehensive care that
          addresses both the physical and emotional well-being of the children
          we serve.
        </p>
        <p class="text-lg mb-6">
          We strongly believe in collaborative partnerships with families,
          communities, and other organizations. By working together, we can make
          a lasting impact on the lives of the children we support. We are
          grateful for the continuous support and generosity of our donors,
          sponsors, and volunteers who share our vision and contribute to our
          mission.
        </p>
        <p class="text-lg mb-6">
          Join us on this incredible journey of transforming lives! Whether
          you'd like to volunteer your time, make a donation, or simply learn
          more about our programs, we invite you to be a part of Sunshine
          Childcare NGO.
        </p>
        <p class="text-lg mb-6">
          Together, we can bring smiles and create brighter futures for the
          children in our care. Thank you for your support!
        </p>
        <p class="text-lg font-semibold">The Sunshine Childcare Team</p>
      </div>
    </div>
  </section>

  <!-- Contact Us section -->
  <section id="contact-us" class="w-full md:flex pc-8 shadow-lg bg-white">
    <div class="md:w-1/2 flex flex-col items-center justify-center py-6">
      <h1 class="font-semibold mb-2">Adress</h1>
      <address class="text-lg">Korem</address>
      <h1 class="font-semibold mb-2 mt-4">Email</h1>
      <p class="text-lg">sunshine@gmail.com</p>
      <h1 class="font-semibold mt-4 mb-2">Tel</h1>
      <p class="text-lg">0929457007</p>
    </div>
    <div class="md:w-1/2 flex flex-col items-center justify-center py-6">
      <h1 class="font-bold text-lg mb-2">Sene us a message</h1>
      <form action="" class="flex flex-col">
        <label for="email" class="font-semibold">Email:</label>
        <input type="text" placeholder="email" class="border border-blue-500 px-2 py-1 mt-1 rounded" v-model="contact.email"/>
        <label for="message" class="font-semibold mt-4">Message:</label>
        <textarea
          name=""
          id="message"
          cols="30"
          rows="10"
          placeholder="message"
          class="border border-blue-500 px-2 py-1 mt-1 rounded" v-model="contact.message"
        ></textarea>
        <button class="bg-green-500 text-white px-4 py-2 mt-4 rounded">
          Submit
        </button>
      </form>
    </div>
  </section>

  <!-- Donation Modal section -->
  <div id="modal" class="fixed h-screen inset-0 z-50 bg-black/20 flex items-center justify-center" v-if="showModal">
    <form action="" class="flex flex-col bg-gray-50 w-1/4 p-8 space-y-3">
      <label for="name">Full Name:</label>
      <input type="text" placeholder="" class="border border-blue-500" v-model="form.fullName"/>
      <label for="amount">Amount:</label>
      <input type="number" id="amount"  class="border border-blue-500" v-model="form.amount"/>
      <button class="bg-green-500 text-white pv-4 py-2 ">Submit</button>
      <button @click="showModal=!showModal">Cancel</button>
    </form>
  </div>

  <!-- footer section -->
  <footer class="bg-gray-900 text-white py-4 px-8" >
    <div class="container mx-auto flex flex-col md:flex-row md:justify-between md:items-center">
      <div>
        <h2 class="text-lg font-semibold">Sunshine Childcare NGO</h2>
        <p class="mt-2">Providing exceptional care and support to children in need</p>
      </div>
      <div>
        <h3 class="text-lg font-semibold">Contact Us</h3>
        <ul class="mt-2">
          <li>Email: sunshine@gmail.com</li>
          <li>Phone: 0929457007</li>
          <li>Address: Hashenge</li>
        </ul>
      </div>

      <div>
        <h3 class="text-lg font-semibold">Follow Us</h3>
        <ul class="mt-2">
          <li><a href="#" class="hover:text-yellow-500">Facebook</a> </li>
          <li><a href="#" class="hover:text-yellow-500">Twitter</a> </li>
          <li>  <a href="#" class="hover:text-yellow-500">Instagram</a> </li>
        </ul>
      </div>
    </div>
  </footer>
  <!-- Small Device Menu Section -->
  <section v-if="showMenu" class="fixed inset-0 bg-black/30 h-full z-50 pt-8 flex justify-end" id="navSmall">
    <ul class="flex flex-col items-center bg-gray-50 w-3/4">
      <li class="px-4 py-2"><router-link to="/">Home</router-link></li>
      <li class="px-4 py-2"><router-link to="#events">Events</router-link></li>
      <li class="px-4 py-2"><router-link to="#about-us">About Us</router-link></li>
      <li class="px-4 py-2"><router-link to="#contact-us">Contact Us</router-link></li>

      <li class="px-4 py-2 bg-yellow-500 text-white"><button @click="showModal = !showModal">Donate Now</button></li>
      <li class="px-4 py-2 bg-gray-500 text-white mt-4"><button @click="showMenu = !showMenu">Cancel</button></li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "HomeView",
  components: {},
  data() {
    return {
      showMenu: false,
      showModal: false,
      form: {

      },
      contact:{}
    };
  },
};
</script>

<style scoped>
.animate-card {
  animation: slide-left 1s ease-in-out forwards;
}
@keyframes slide-left {
  0% {
    transform: translate(80px, -150px);
  }
  100% {
    transform: translate(30px, 0);
  }
}
</style>
