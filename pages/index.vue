<template>
  <div>
    <div class="mainVisual"></div>

    <section class="primarySection">
      <div class="container">
        <h2 class="primaryHeading">about</h2>
        <div class="profile">
          <div class="profile__upper">
            <div class="profile__text">
              <p class="profile__name">
                山田 太郎<span lang="en">Taro Yamada</span>
              </p>
              <dl class="profile__item">
                <dt class="profile__title">技術スタック</dt>
                <dd>HTML / CSS / jQuery / JavaScript / Nuxt</dd>
              </dl>
              <dl class="profile__item">
                <dt class="profile__title">趣味</dt>
                <dd>開発、ゲーム、YouTube、ライブ、音楽フェス、ピアノ、卓球</dd>
              </dl>
            </div>
            <figure class="profile__image">
              <img src="https://placehold.jp/260x260.png" alt="your name" />
            </figure>
          </div>
          <p>
            自己紹介を入れましょう。出身や経歴と現在の仕事の内容を簡単に話すも良し。<br />数年後の目標や今学んでいること、活動している内容を入れるのも良いかと思います。
          </p>
        </div>
      </div>
    </section>

    <section class="primarySection background--gray">
      <div class="container container--lg">
        <h2 class="primaryHeading">works</h2>
        <ol>
          <li>
            <figure>
              <img src="https://placehold.jp/540x334.png" alt="" />
            </figure>
            <div>
              <p>作品名</p>
              <p><time datetime="2021.12.16">2021.12.16</time></p>
            </div>
          </li>
        </ol>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style lang="scss" scoped>
.profile {
  &__upper {
    display: flex;
    flex-direction: column-reverse;
    margin-bottom: 0.5em;

    @include mq() {
      flex-direction: row-reverse;
      justify-content: space-between;
      margin-bottom: 2em;
    }
  }

  &__text {
    @include mq() {
    }
  }

  &__name {
    font-size: fz(24);
    font-weight: bold;
    margin-bottom: 0.5em;

    @include mq() {
      font-size: fz(28);
      margin-bottom: 0.857em;
    }

    [lang='en'] {
      font-size: fz(18);

      &::before {
        content: '/';
        margin: 0 0.5em;
      }
    }
  }

  &__item {
    margin-bottom: 0.5em;

    @include mq() {
      margin-bottom: 1em;
    }
  }

  &__title {
    font-size: fz(18);
    font-weight: bold;
    margin-bottom: 0.222em;

    @include mq() {
      margin-bottom: 0.444em;
    }
  }

  &__image {
    width: 100%;
    margin-bottom: 1.75em;

    @include mq() {
      width: 40%;
      margin: 0 2em 0 0;
    }

    img {
      width: 100%;
    }
  }
}
</style>
