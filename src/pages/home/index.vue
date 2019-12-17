<template>
<div>
  <div class="header">
      <span>豆瓣</span>
      <icon type="search" size="16" color="#00b600"></icon>
      <button>打开豆瓣App</button>
  </div>
  <div class="movie-item">
 <p class="title">
        <span>影院热映</span>
        <span class="more-like">更多</span>
      </p>
      <scroll-view class="scroll-view_H" scroll-x="true" style="width: 100%">
         <div class="scroll-view-item_H" v-for="(item,index) in 5" :key="index">
            <img src="https://img3.doubanio.com/view/photo/m/public/p2576090251.webp" alt="">
        <span>天地对决</span>
         <div class="rating">
           <div class="stars">
       <!-- <img src="" alt=""> -->
           </div>
           <span>6.3</span>
         </div>
         <div>hihihiu</div>
               <div>hihihiu</div>
                     <div>hihihiu</div>
                      
         </div>
        </scroll-view>
  </div>
</div>

  
</template>

<script>
export default {

}
</script>

<style lang="less">
.header{
  height: 94rpx;
  border-bottom: 1rpx solid #eee;
  display: flex;
  padding: 0 36rpx;
  align-items: center;
   span {
    color: #00b600;
    font-size: 40rpx;
  }
  icon {
    flex: 1;
    margin-left: 28rpx;
  }
  button {
    background-color: #42bd56;
    color: #fff;
    width: 200rpx;
    height: 58rpx;
    border-radius: 8rpx;
    line-height: 58rpx;
    font-size: 24rpx;
  }
}
.movie-item {
  .title {
    height: 88rpx;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 36rpx;
    .more-like {
      color: #42bd42;
    }
  }
}
.scroll-view_H {
  display: flex;
  white-space: nowrap;
}
.scroll-view-item_H {
 
  display: inline-block;
  img{
    width:200rpx;
    height: 286rpx;;
  }
}
</style>