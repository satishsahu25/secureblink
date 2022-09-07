<template>
  <div class="singleitem">
    <p>
      It's a comprehensive online learning platform for everyone looking to
      learn and course pro. provinding this platform which is very beneficial
      for practicals. Students can revise everything at home like dissection and
      slides
    </p>
    <div class="desc">
      <div class="leftd">
        <img
          src="../../assets/christopher-campbell-rDEOVtE7vOs-unsplash.png"
          alt=""
        />
        <div class="name">
          <span class="tname">{{ testit.name }}</span><br>
          <span class="ttime">Yesterday</span>
        </div>
      </div>
      <div class="rightd">
        <img src="../../assets/right-quotation-sign.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    testit: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.singleitem {
  flex: 1;
  border-radius: 10px;
  margin: 1rem;
  padding-bottom: 2rem;
  -webkit-box-shadow: 5px 5px 5px 5px #00000057;
  box-shadow: 0px 2px 10px 10px #0000001f;
}
.singleitem p {
  padding: 2rem;
}

.leftd img {
  border-radius: 50%;
  height: 2rem;
  width: 2rem;
}
.desc {
  padding: 0.5rem 1rem;
  display: flex;
  justify-content: space-between;
}
.leftd {
  display: flex;
}
.rightd {
  height: 2rem;
  width: 2rem;
  padding-right: 5rem;
}
.leftd .name {
  margin-left: 0.5rem;
}
.leftd .name .tname {
  font-weight: bold;
  color: black;
}
.leftd .name .ttime{
    color: #545d7a;
}
</style>
