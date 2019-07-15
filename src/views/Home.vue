<template>
  <div class="main">
    <div class="input">
      <input
        type="text"
        placeholder="ADD A NEW MISSION…"
      ></div>
    <div class="toDoList">
      <div
        class="list"
        v-for="(item, index) in list"
        :key="index"
      >
      <div class="listDot"></div>
        <div class="listTitle">{{item.title}}</div>
      </div>
    </div>
    <div class="timing-container">
      <div class="timing-cpntent">
        <div class="play"></div>
        <div class="give-up"></div>
      </div>
    </div>

    <div class="nav-container">
      <nav class="nav-list">
        <li>
          <i class="material-icons">list</i>
          <!-- <span>to-do list</span> -->
        </li>
        <li><i class="material-icons">insert_chart</i>
          <!-- <span>analytics</span> -->
        </li>
        <li><i class="material-icons">library_music</i>
          <!-- <span>ringtones</span> -->
        </li>
      </nav>
      <div class="logo">POMODORO</div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  data() {
    return {
      list: [
        { title: 'the First thing to do today', status: false, time: 2000 },
        { title: 'the second thing to do today', status: false, time: 2000 },
        { title: 'the third thing to do today', status: false, time: 2000 },
        { title: 'the forth thing to do today', status: false, time: 2000 },
      ]
    }
  }
}
</script>

