<template>
  <div class="hero-text">
    <h1>Hello</h1>
    <p>i am a copy writer</p>
    <button>Get my resume</button>
  </div>
</template>

<style scoped>
.hero-text {
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  background: linear-gradient(to right, #a3c9d6, #6eb8d1);
  max-width: 100%;
  height: 450px;
  margin: 30px;
  align-items: center;
  border-radius: 8px;
  color: rgb(29, 27, 27);
  
}

h1 {
  font-size: 9em;
  font-weight: 600;
}

p{
  font-size: 2rem;
  letter-spacing: 2px;
  text-transform: capitalize;
}

button {
  margin: 15px ;
  padding: 15px 20px;
  border: 2px solid #000;
  background: #ffffff;
  color: rgb(29, 27, 27);
  font-size: 18px;
  font-weight: 600;
  text-transform: uppercase;
  cursor: pointer;
  box-shadow: 4px 5px 0px rgba(0, 0, 0, 0.99);
}

button:hover {
  box-shadow: 0 0 0 rgba(0, 0, 0, 0.00);
}

@media (max-width: 768px) {
  .hero-text {
    padding: 10px;
    max-width: 100%;
  }

  h1 {
    font-size: 5em;
  }


}

/* @media (max-width: 320px) {
  h1 {
    font-size: 3em;
  }
  
  p {
    font-size: 1.5em;
  }

  button {
    display: block;
    padding: 15px;
    font-size: 10px;
  }

} */

</style>