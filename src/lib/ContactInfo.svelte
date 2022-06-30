<script>

const team = [
  { name: "Joe Burrow", img: '../public/images/joe.jpeg', github: 'https://github.com/jmborrow', linkedin:'https://www.linkedin.com/in/joe-borrow/', id: 1},
  { name: "Celena Chan", img: '../public/images/celena.jpeg', github: 'https://github.com/celenachan', linkedin:'https://www.linkedin.com/in/celenachan/', id: 2},
  { name: "Aaron Dreyfuss", img: '../public/images/aaron.png', github: 'https://github.com/AaronDreyfuss7', linkedin:'https://www.linkedin.com/in/aaron-dreyfuss-708b9bb4/', id: 3},
  { name: "Hank Jackson", img: '../public/images/hank.png', github: 'https://github.com/hankthetank27', linkedin:'https://www.linkedin.com/in/hank-jackson-10345317/', id: 4},
  { name: "Jasper Narvil", img: '../public/images/jasper2.jpg', github: 'https://github.com/jnarvil3', linkedin:'https://www.linkedin.com/in/jaspernarvil/', id: 5},
]
</script>

<div class="contact">
  <ul class="contactlist">
    {#each team as member}
      <img src={member.img} alt='{member.name} photo'>
      <!-- <center> -->
       {member.name}
      <img id="github" src='../public/images/github.png' alt='github'>
      <img id="linkedin" src='../public/images/linkedin.png' alt='linkedin'>
      <!-- </center> -->
      
    {/each}
    
  </ul>

</div>

<style>
  
  .contact {
    display: flex;
    flex-wrap: wrap;
    /* flex-direction: column; */
    /* align-items: center; */
  }

  .contactlist {
    color: white;
  }

  img {
    width: 150px;
    border-radius: 75px;

  }

  #github, #linkedin {
    width:30px;

  }
</style>