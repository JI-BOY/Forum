<script>
import SideBarRightSearch from '@/components/SideBarRight/SideBarRightSearch'
import Icons from '@/components/Icons'

export default {
  components: {
    SideBarRightSearch,
    Icons
  }
}
</script>

<template>
  <div class="side-bar-right-trend">
    <side-bar-right-search />
    <div class="trends">
      <div class="title">
        <span>为您推荐</span>
        <icons icon="settings" />
      </div>
      <!-- <div class="trend">
        <div class="content">
          <p class="rank">Politics · Trending</p>
          <h4 class="caption">#istanbulsozlesmesiyasatir</h4>
          <p class="tweet-number">82M Tweets</p>
        </div>
        <icons icon="three-dot" class="section" />
      </div> -->
      <!-- <div class="trend">
        <div class="content">
          <p class="rank">Politics · Trending</p>
          <h4 class="caption">#ırkcılık</h4>
          <p class="tweet-number">40M Tweets</p>
        </div>
        <icons icon="three-dot" class="section" />
      </div>
      <div class="trend">
        <div class="content">
          <p class="rank">Politics · Trending</p>
          <h4 class="caption">#adalet</h4>
          <p class="tweet-number">70M Tweets</p>
        </div>
        <icons icon="three-dot" class="section" />
      </div>
      <div class="trend">
        <div class="content">
          <p class="rank">Politics · Trending</p>
          <h4 class="caption">#128milyardolarnerede</h4>
          <p class="tweet-number">40M Tweets</p>
        </div>
        <icons icon="three-dot" class="section" />
      </div>
      <div class="trend">
        <div class="content">
          <p class="rank">Politics · Trending</p>
          <h4 class="caption">#ekonomi</h4>
          <p class="tweet-number">100M Tweets</p>
        </div>
        <icons icon="three-dot" class="section" />
      </div>
      <div class="trend">
        <div class="content">
          <p class="rank">Politics · Trending</p>
          <h4 class="caption">#egitim</h4>
          <p class="tweet-number">46M Tweets</p>
        </div>
        <icons icon="three-dot" class="section" />
      </div> -->
      <div class="nocontent">
        暂无推荐
      </div>
      <h4 class="show-more"><svg t="1676255340354" class="icon" viewBox="0 0 1024 1024" version="1.1"
          xmlns="http://www.w3.org/2000/svg" p-id="6891" width="16" height="16">
          <path
            d="M640 921.6V981.333333l-85.333333-85.333333-42.666667-42.666667h21.333333c174.933333 0 320-145.066667 320-320 0-145.066667-93.866667-264.533333-226.133333-307.2L571.733333 170.666667c183.466667 21.333333 324.266667 174.933333 324.266667 358.4 0 174.933333-123.733333 320-290.133333 354.133333l34.133333 38.4zM426.666667 145.066667V85.333333l85.333333 85.333334 42.666667 42.666666h-21.333334C358.4 213.333333 213.333333 354.133333 213.333333 533.333333c0 140.8 93.866667 264.533333 221.866667 302.933334l55.466667 55.466666c-179.2-21.333333-320-170.666667-320-358.4C170.666667 358.4 294.4 213.333333 460.8 179.2l-34.133333-34.133333z"
            fill="#1da1f2" p-id="6892"></path>
        </svg>换一批</h4>
    </div>
  </div>
</template>

<style scoped lang="scss">
.side-bar-right-trend {
  max-width: 350px;
  width: 350px;
  margin-top: 0.2rem;
  margin-bottom: 24px;
  margin-left: 25px;
  display: flex;
  flex-direction: column;
  justify-content: center;

  .nocontent {
    height: 100px;
    line-height: 100px;
    background-color: #f6f8fa;
    color: #000;
    font-size: 14px;
    text-align: center;
  }

  .trends {
    display: flex;
    flex-direction: column;
    border-radius: 12px;
    background: #f6f8fa;
    position: sticky;
    top: 15px;

    .title {
      padding: 4px 16px;
      display: flex;
      cursor: pointer;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid rgba(0, 0, 0, 0.08);
      padding-bottom: 12px;
      font-weight: 800;

      span {
        font-weight: 900;
        font-size: 20px;
        line-height: 22.27px;
        color: #000;
      }

      svg {
        width: 22px;
        height: 22px;
        padding: 0.5rem;
        box-sizing: content-box;
        border-radius: 50%;

        &:hover {
          background-color: rgba(#1da1f2, 0.2);
        }
      }
    }

    .trend {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      cursor: pointer;
      border-bottom: 1px solid rgba(0, 0, 0, 0.08);
      padding-bottom: 0.5rem;
      padding-top: 0.5rem;
      padding-left: 20px;
      padding-right: 20px;

      .section {
        border-radius: 50%;
        box-sizing: content-box;
        padding: .5rem;

        &:hover {
          background-color: rgba(#1da1f2, 0.1);
          fill: #1da1f2;
        }
      }

      .content {
        display: flex;
        flex-direction: column;
        align-items: flex-start;

        * {
          margin-bottom: 4px;
        }

        .rank {
          line-height: 14px;
          font-size: 12px;
          font-weight: 400;
          color: rgb(91, 112, 131);
        }

        .caption {
          font-size: 15px;
          line-height: 17.58px;
          font-weight: 700;
          color: #333;
        }

        .tweet-number {
          font-size: 14px;
          line-height: 16.41px;
          color: rgb(91, 112, 131);
        }
      }

      &:hover {
        background-color: rgba(0, 0, 0, 0.03);
      }
    }

    h4.show-more {
      color: #1da1f2;
      text-align: center;
      font-weight: 500;
      font-size: 14px;
      line-height: 16.41px;
      cursor: pointer;
      padding: 16px;
      text-align: left;
      font-weight: 300;
      border-bottom-left-radius: 10px;
      border-bottom-right-radius: 10px;

      &:hover {
        background-color: rgba(0, 0, 0, 0.03);
      }
    }
  }
}
</style>