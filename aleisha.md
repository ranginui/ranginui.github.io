<style>
  * {
  box-sizing: border-box;
}

/* Set a background color */
body {
  background-color: #474e5d;
  font-family: Helvetica, sans-serif;
}

/* The actual timeline (the vertical ruler) */
.timeline {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
}

/* The actual timeline (the vertical ruler) */
.timeline::after {
  content: '';
  position: absolute;
  width: 6px;
  background-color: white;
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: -3px;
}

/* Container around content */
.container {
  padding: 10px 40px;
  position: relative;
  background-color: inherit;
  width: 50%;
}

/* The circles on the timeline */
.container::after {
  content: '';
  position: absolute;
  width: 25px;
  height: 25px;
  right: -17px;
  background-color: white;
  border: 4px solid #FF9F55;
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

/* Place the container to the left */
.left {
  left: 0;
}

/* Place the container to the right */
.right {
  left: 50%;
}

/* Add arrows to the left container (pointing right) */
.left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid white;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent white;
}

/* Add arrows to the right container (pointing left) */
.right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid white;
  border-width: 10px 10px 10px 0;
  border-color: transparent white transparent transparent;
}

/* Fix the circle for containers on the right side */
.right::after {
  left: -16px;
}

/* The actual content */
.content {
  padding: 20px 30px;
  background-color: white;
  position: relative;
  border-radius: 6px;
}

/* Media queries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
/* Place the timelime to the left */
  .timeline::after {
    left: 31px;
  }

/* Full-width containers */
  .container {
    width: 100%;
    padding-left: 70px;
    padding-right: 25px;
  }

/* Make sure that all arrows are pointing leftwards */
  .container::before {
    left: 60px;
    border: medium solid white;
    border-width: 10px 10px 10px 0;
    border-color: transparent white transparent transparent;
  }

/* Make sure all circles are at the same spot */
  .left::after, .right::after {
    left: 15px;
  }

/* Make all right containers behave like the left ones */
  .right {
    left: 0%;
  }
}
</style>

<iframe src="https://free.timeanddate.com/countdown/i6w2gs8q/n264/cf110/cm0/cu4/ct0/cs0/ca0/cr0/ss0/cac000/cpc000/pca0bfd5/tcfff/fs100/szw320/szh135/tatTime%20left%20until/tac000/tptTime%20since%20Aleisha%20finished%20Uni/tpc000/matAleisha%20is%20free%20from%20University/mac000/mpc000/iso2019-10-28T18:00:00" allowTransparency="true" frameborder="0" width="320" height="135"></iframe>

 <div class="timeline">
  <div class="container left">
    <div class="content">
      <h2>16/8 Te Rakau nui</h2>
      <p>High Energy, get all your stuff done today Aleisha</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>23/8 Tangāroa-a-mua</h2>
      <p>Another high energy day, you got this Aleisha, smash it out</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>30/8 Whiro</h2>
      <p>Anyone who set an assignment due now was taking the piss</p>
    </div>
  </div>
   <div class="container right">
    <div class="content">
      <h2>6/9 Tamatea-a-aio</h2>
      <p>Stay away from the moana, I know how you could do that, work on your assignments instead!</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>13/9 Oturu</h2>
      <p>High energy day, a good day to finalise decisions today you can pick the wine you will buy for the night of the 28/10</p>
    </div>
  </div>
 <div class="container right">
    <div class="content">
      <h2>20/9 Korekore te piri ki Tangaroa</h2>
      <p>A good day to reinvigorate and reflect/review. You should review your assignments and definitely buy Chris a coffee</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>27/9 Mauri</h2>
      <p>Low energy day, get an extension if stuff is due today. Tell the lecturer "I don't make the rules, the maramataka does" if they argue</p>
    </div>
  </div>
 <div class="container right">
    <div class="content">
      <h2>4/10 Tamatea kai Ariki</h2>
      <p>Plant some food today. Remember to bring in some Oreos for Hayley</p>
    </div>
  </div>
 <div class="container left">
    <div class="content">
      <h2>11/10 Ohua</h2>
      <p>Another good day for working, you can probably get like 6 assignments done today</p>
    </div>
  </div>
 <div class="container right">
    <div class="content">
      <h2>18/10 Korekore te whīwhīa</h2>
      <p>Just forget about it, this day is a write off. Go to beer o'clock instead</p>
    </div>
  </div>
 <div class="container left">
    <div class="content">
      <h2>25/10 Otane</h2>
      <p>High energy day, and a day for giving back. Give back that last assignment 3 days early</p>
    </div>
  </div>
 <div class="container right">
    <div class="content">
      <h2>28/10 Whiro</h2>
      <p>Embrace the chaos of Whiro. Drinks are on Chris, Amber and Kris. You're finished! And we all couldn't be prouder of you.</p>
    </div>
  </div>
</div> 

<p> Disclaimer: this is my limited understanding of the maramataka adapted for this purpose</p>

