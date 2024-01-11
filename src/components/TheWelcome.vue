<template>
  <div class="hero-text">
    <h1>Hello</h1>
    <p>i am a copy writer</p>
    <button>Get my resume</button>
  </div>
</template>

<style scoped>
.hero-text {
  background: linear-gradient(to right, #a3c9d6, #6eb8d1);
  max-width: 100%;
  padding: 20px;
  margin: 30px 40px;
  text-align: center;
  border-radius: 8px;
  color: rgb(29, 27, 27);
  
}

h1 {
  font-size: 9rem;
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
</style>