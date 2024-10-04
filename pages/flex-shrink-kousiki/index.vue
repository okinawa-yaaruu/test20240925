<template>

  <p>全体の幅は 500px で、フレックスアイテムの flex-basis は 120px です。</p>
  <p>A、B、C には flex-shrink:1 が、D と E には flex-shrink:2 が設定されています。</p>
  <p>D と E の幅は他より狭くなります。</p>
  <p>結局、120*5-500=100px足りない。なので、100/(1+1+1+2+2)=約14.28pxになり</p>
  <p>flex-shrink:1のdiv幅は120-14.28=105.72px</p>
  <p>flex-shrink:2のdiv幅は120-(14.28*2)=91.44だが、</p>
  <p>全部足すと500.04なってしまうので、0.04をflex-shrink:2のdivから引くので</p>
  <p>flex-shrink:2のdiv幅は120-(14.28*2)-0.02=91.42</p>
  <div id="content">
    <div class="box" style="background-color:red;">A</div>
    <div class="box" style="background-color:lightblue;">B</div>
    <div class="box" style="background-color:yellow;">C</div>
    <div class="box1" style="background-color:brown;">D</div>
    <div class="box1" style="background-color:lightgreen;">E</div>
  </div>

</template>
<style scoped>
#content {
  display: flex;
  width: 500px;
}

#content div {
  flex-basis: 120px;
  /* border: 3px solid rgba(0, 0, 0, 0.2); */
}

.box {
  flex-shrink: 1;
}

.box1 {
  flex-shrink: 2;
}
</style>