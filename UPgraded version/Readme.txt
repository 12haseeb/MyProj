* Speakers */

.speakers {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  flex-direction: column;
  /* To be changed */
  height: 40vh;
  position: relative;
  box-sizing: border-box;
  background: radial-gradient(
    circle,
    #2a2b2d9d 0%,
    #2a2b2d 81%,
    rgba(255, 94, 0, 1) 100%
  );
  overflow: auto;
}

/* Button : See More  */
.btn {
  cursor: pointer;
  border: 2px outset #ff5e00;
  box-shadow: 1px 1px 2px #FF5E00;
  text-shadow: 1px 1px 0px #393939;
  border-radius: 20px;
  padding: 10px 30px;
  background: transparent;
  font-size: 15px;
  text-transform: uppercase;
  font-weight: bold;
  /* align-self: center; */
}

.btn a{
  text-decoration: none;
  color:  #0067B8 !important;
}

.btn i{
  width: 30px;
  padding: 10px;
  box-sizing: border-box;
}

.btn:hover i{
  width: 30px;
  padding-left: 15px;
  box-sizing: border-box;
}

.speakers .speaker {
  /* background-color: #eee; */
  height: 30vh;
  width: 19%;
  justify-content: center;
  position: relative;
  margin: 0px 25.3px ;
  z-index: 1;
}

/* Box shadow will be applied when hover on each image. */
/* Re-arranging the lines of code with the help of selectors. */
.iad img {
  object-position: 0px -80px;
  box-shadow: 0px 0px 0px 0px #2a2b2d, 0px 0px 0px 0px #8f8d8d;
  transition: box-shadow 1s ease;
}
.im img,
.sa img {
  object-position: 0px 0px;
  box-shadow: 0px 0px 0px 0px #2a2b2d, 0px 0px 0px 0px #7c7c7c;
  transition: box-shadow 1s ease;
}

.iad:hover img,
.im:hover img {
  box-shadow: 4px 0px 7px 1px #ff5e00, -4px 0px 7px 1px #8f8d8d;
}

.sa:hover img {
  box-shadow: 4px 0px 7px 1px #7c7c7c, -4px 0px 7px 1px #ff5e00;
}

.speakers .speaker img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ensures image covers full div */
  position: absolute; /* Ensures full stretch */
  top: 0;
  left: 0;
  z-index: 1;
}

.speakers .speaker-info {
  border: 1px outset rgb(162, 162, 162);
  background-color: #2a2b2d65;
  height: calc(100% - 2px);
  /* padding: 10px; */
  text-align: justify;
  overflow: auto;
  box-sizing: border-box;
  padding: 0px 10px;
  line-height: 1.3;
  justify-items: center;
  position: absolute;
  top: 0pc;
  left: 0;
  z-index: 0;
}
.speakers .speaker-info p {
  font-family: "Roboto", sans-serif;
  font-size: 16px;
}

/* To apply transition on all of the img seperately, we have to style each of them with specified classes by giving them transition property. */
/* Apply the transition first for all the images seperately */

.speaker .iad-2,
.speaker .im-2,
.speaker .sa-2 {
  transform: translateX(0); /* Initial position */
  transition: transform 1s ease; /* Smooth transition */
}

/* Hover classes */
.speaker:hover .iad-2,
.speaker:hover .im-2 {
  transform: translateX(103%);
}

.speaker:hover .sa-2 {
  transform: translateX(-103%);
}

.speakers .speaker-info h1 {
  color: #ff5e00;
  text-shadow: 1px -2px 2px #9e9d9d;
}

.speakers .speaker-info h3 {
  color: #9e9d9d;
  /* text-shadow: 1px -2px 3px rgba(255, 255, 255, 0.46); */
}

/* VENUE */

/* Animation For the 'Speakers' Part */
@keyframes AbtSpkr-Anim {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(100px);
  }
}
