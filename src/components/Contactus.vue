<template>
  <div class="contact">
    <h3>Contact Us</h3>
    <h2>Reach Out With Any <br>Question You Have</h2>
    <div class="contactarea">
      <div class="leftc">
        <h2>Contact Information</h2>
        <div class="item">
          <img src="../assets/whitemail.svg" alt="" />
          <p>contact@coursepro.com</p>
        </div>
        <div class="item">
          <img src="../assets/whitephone.svg" alt="" />
          <p>1800-562-895, 1800-869-877</p>
        </div>
        <div class="item">
          <img src="../assets/whiteloc.svg" alt="" />
          <p>102 Street, India</p>
        </div>
        <h2 class="foot">Social Media Channel</h2>
          <div class="leftf">
            <img src="../assets/Facebook.svg" alt="" />
            <img src="../assets/twitter.svg" alt="" />
            <img src="../assets/Github.svg" alt="" />
            <img src="../assets/Linkedin.svg" alt="" />
        </div>
      </div>
      <div class="rightc">
        <h2>
          Fill up the form and our team will get back to you within 24 hours
        </h2>
        <div class="fillups">
          <div class="first">
            <input type="text" placeholder="Name" />
            <input type="text" placeholder="Email" />
          </div>
          <div class="second">
            <input type="text" placeholder="Phone" />
            <input type="text" placeholder="Subject" />
          </div>
          <textarea
            name=""
            id=""
            cols="30"
            rows="10"
            placeholder="Message"
          ></textarea>
          <button class="submitbtn">Submit</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>

.contact .contactarea {
  display: flex;
  margin-top: 5rem;
  text-align: center;
}
.contact .contactarea .leftc {
  flex: 1;
}
.contact h3 {
  font-style: italic;
  font-weight: normal;
  font-size: 20px;
  color: #01cb63;
  text-align: center;
}
.contact h2 {
  /* margin-top: 5rem; */
  text-align: center;
  font-weight: 600;
  font-size: 25px;
}
.contact .contactarea .rightc {
  flex: 1;
  padding: 5rem;
  margin-top: -5rem;
}
.contact .contactarea .leftc p {
  font-weight: 500;
  font-size: 20px;
}
.contact .contactarea .leftc img {
  height: 5rem;
  width: 5rem;
  margin: 0.1rem 0.5rem;
  border-radius: 50%;
}
.contact .contactarea .leftc div {
  display: flex;
  align-items: center;
  margin-left: 12rem;
}
  .leftf {
  display: flex;
}
.leftf img{
  scale: 0.6;
  object-fit: cover;
}
.fillups {
  text-align: center;
  padding: 2rem;
}
.fillups button {
  margin-top: 1rem;
  color: white;
  background-color: black;
  font-style: italic;
  border-radius: 5px;
  padding: 0.5rem 4rem;
}
.first {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.first input {
  font-size: 20px;
  border: none;
  outline: none;
  padding: 0.5rem 0.2rem;
  border-bottom: 3px solid #01cb63;
}
.second {
  display: flex;
  margin-top: 1rem;
  align-items: center;
  justify-content: space-between;
}
.second input {
  border: none;
  font-size: 20px;
  outline: none;
  padding: 0.5rem 0.2rem;
  border-bottom: 3px solid #01cb63;
}
textarea {
  margin-top: 1rem;
  outline: none;
  font-size: 20px;
  border: 3px solid #01cb63;
  resize: vertical;
  width: 100%;
  padding: 0.5rem 0.2rem;
}
@media only screen and (max-width:1200px){
.contactarea{
  flex-direction: column;
}
.contactarea .leftc{
  text-align: center;
  justify-content: center;
}
.rightc .fillups{
  flex-direction: column;
}
.first{
  flex-direction: column;
}
.first input{
  width: 100%;
}
.second{
  flex-direction: column;
}
.second input{
  width: 100%;
}
}
@media only screen and (max-width:960px){
    .leftc .item{
      text-align: start;
    }
    .contact .contactarea .leftc div {
      display: flex;
  text-align: center;
  margin-left: 2rem;
}
    }
</style>
