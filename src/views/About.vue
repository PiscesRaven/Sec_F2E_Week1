<template>
  <div class="pomodoro">
    <nav class="sideNav">
      <a>
        <i class="material-icons">list</i>
      </a>
      <a><i class="material-icons">insert_chart</i>
      </a>
      <a><i class="material-icons">library_music</i>
      </a>
      <a><i class="material-icons">library_music</i>
      </a>
      <a><i class="material-icons">music_note</i>
      </a>
    </nav>
    <div class="toDoList">
      <div class="listTitle">TO DO LIST</div>
      <nav class="list">
        <li class="content">
          <span>The first thing to do</span>
          <div class="contentPlay"></div>
        </li>
      </nav>
      <div class="timingContainer"></div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
@import "../assets/css/mixin.scss";
.pomodoro {
  @include size(100%, 937px);
  .sideNav {
    @include size(130px, 100%);
    background: linear-gradient(to bottom, #15a9b6 0%, #10767e 100%);
    padding-top: 550px;
    float: left;
    a {
      cursor: pointer;
      display: block;
      padding: 32px 0;
      i {
        color: #18c4d3;
      }
    }
  }
  .toDoList {
    @include size(470px, 100%);
    text-align: left;
    float: left;
    padding-top: 220px;
    padding-left: 100px;
    color: #3aabb4;
    .listTitle {
      @include size(315px, 54px);
      line-height: 54px;
      text-transform: uppercase;
      font-weight: 700;
    }
    .list {
      @include size(315px, 54px);
      .content {
        // background: linear-gradient(
        //   to bottom,
        //   #3f9ae3 0%,
        //   #349cc8 1%,
        //   #3aabb4 2%,
        //   #3aabb4 100%
        // );
        span {
          color: #3aabb4;
          line-height: 24px;
        }
        .contentPlay {
          @include size(30px);
          @include setBorder(1px, #3aabb4);
          position: relative;
          border-radius: 50%;
        }
      }
    }
  }
}
</style>
