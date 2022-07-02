<script>

const team = [
  { name: "Joe Borrow", img: '../public/images/joe.jpeg', github: 'https://github.com/jmborrow', linkedin:'https://www.linkedin.com/in/joe-borrow/', id: 1},
  { name: "Celena Chan", img: '../public/images/celena.jpeg', github: 'https://github.com/celenachan', linkedin:'https://www.linkedin.com/in/celenachan/', id: 2},
  { name: "Aaron Dreyfuss", img: '../public/images/aaron.png', github: 'https://github.com/AaronDreyfuss', linkedin:'https://www.linkedin.com/in/aaron-dreyfuss-708b9bb4/', id: 3},
  { name: "Hank Jackson", img: '../public/images/hank.png', github: 'https://github.com/hankthetank27', linkedin:'https://www.linkedin.com/in/hank-jackson-10345317/', id: 4},
  { name: "Jasper Narvil", img: '../public/images/jasper3.jpg', github: 'https://github.com/jnarvil3', linkedin:'https://www.linkedin.com/in/jaspernarvil/', id: 5},
]
</script>

<a id="#contactLink">
<div class="contact">
  <span class="contactTitle">
    <i>
      <span>
        Meet the Team
      </span>
    </i>
  </span>

  {#each team as member}
    <div>
    <img src={member.img} alt='{member.name} photo'><br>
      <center><b>
        {member.name}
      </b>
      <br>
      <a href={member.github}><img id="github" src='../public/images/github.png' alt='github'><!--
      --><a href={member.linkedin}><img id="linkedin" src='../public/images/linkedin.png' alt='linkedin'>
      </center>
    </div>
  {/each}
</div>
</a>


<style>

  div {
    /* background-color: #6E896A; */
    padding: 50px;
    /* margin-top: 150px;
    margin-bottom: 150px; */
    /* border: 150px;
    border-color: 150px; */
  }
  
  .contact {
    display: flex;
    /* align-items: center; */
    justify-content: space-evenly;
    color: white;
    flex-wrap: wrap;
    /* margin-top: 200px; */
  }

  .contactTitle {
  font-size: 3em;
  width: 100%;
  color: white;
  text-shadow: 2px 2px 4px;
  text-align: center
}

  img {
    width: 150px;
    border-radius: 75px;
    border: 2px solid white;
  }

  img:hover {
    animation: shake 0.5s;
    animation-iteration-count: infinite;
  }


  @keyframes shake {
  0% { transform: translate(1px, 1px) rotate(0deg); }
  10% { transform: translate(-1px, -2px) rotate(-1deg); }
  20% { transform: translate(-3px, 0px) rotate(1deg); }
  30% { transform: translate(3px, 2px) rotate(0deg); }
  40% { transform: translate(1px, -1px) rotate(1deg); }
  50% { transform: translate(-1px, 2px) rotate(-1deg); }
  60% { transform: translate(-3px, 1px) rotate(0deg); }
  70% { transform: translate(3px, 1px) rotate(-1deg); }
  80% { transform: translate(-1px, -1px) rotate(1deg); }
  90% { transform: translate(1px, 2px) rotate(0deg); }
  100% { transform: translate(1px, -2px) rotate(-1deg); }
}

  #github, #linkedin {
    width:30px;
  }
</style>