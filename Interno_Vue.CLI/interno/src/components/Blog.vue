<template>
          <section class="intro">
            <div class="intro__content">
                <div class="intro__title-content">
                    <h2 class="intro__heading">Articles & News</h2>
                    <ul class="intro__breadcrumbs">
                        <li class="intro__breadcrumbs-item">
                                      <!-- ????????? -->
                            <a href="../index.html" class="intro__breadcrumbs-link">Home</a>
                        </li>
                        <li class="intro__breadcrumbs-item">
                            <a href="#" class="intro__breadcrumbs-link">Blog</a>
                        </li>
                    </ul>
                </div>
            </div>
        </section>
        <section class="post center">
            <div class="post__content">
                <h2 class="post__heading">Latest Post</h2>
                <div class="post__subcontent-box">
                    <img src="../assets/images/blog_post.png" alt="post image">
                    <article class="post__subcontent">
                        <div class="post__subcontent-container">
                            <h3 class="post__subcontent-heading">Low Cost Latest Invented Interior Designing Ideas</h3>
                            <p class="post__subcontent-text">Lorem ipsum dolor sit amet, adipiscing Aliquam eusem vitae turpis dignissim maximus.posuere in. Contrary to popular belief.</p>
                            <p class="post__subcontent-text">Lorem Ipsum is not simply random text. It has roots in a piece of classica.</p>
                        </div>
                        <div class="post__subtitle-box">
                            <p class="post__subcontent-subtitle">26 December,2022</p>
                            <button class="post__button">
                                <svg
                                    width="9"
                                    height="16"
                                    viewBox="0 0 9 16"
                                    fill="none"
                                    xmlns="http://www.w3.org/2000/svg"
                                >
                                    <path
                                        d="M1.27101 14.9525L7.21387 8.26683L1.27101 1.58112"
                                        stroke="#292F36"
                                        stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                    />
                                </svg>
                            </button>
                        </div>
                    </article>
                </div>
            </div>
        </section>
        <section class="news center">
            <div class="news__content">
                <h2 class="news__heading">Articles & News</h2>
                <div class="news__items" >
                    <div v-for="item in itemsData" :key="item.id" class="news__item">
                        <img :src="item.src" :alt="item.alt" class="news__item-image">
                        <div class="news__item-tagbox">
                            <p class="news__item-tag">{{item.tag}}</p>
                        </div>
                        <div class="item-content">
                            <p class="item-content__title">{{item.title}}</p>
                            <div class="item-content__box">
                                <p class="item-content__date">{{item.date}}</p>
                                <a href="blog-details.html" class="item-content__button">
                                    <svg
                                        width="9"
                                        height="16"
                                        viewBox="0 0 9 16"
                                        fill="none"
                                        xmlns="http://www.w3.org/2000/svg"
                                    >
                                        <path
                                            d="M1.27101 14.9525L7.21387 8.26683L1.27101 1.58112"
                                            stroke="#292F36"
                                            stroke-width="2"
                                            stroke-linecap="round"
                                            stroke-linejoin="round"
                                        />
                                    </svg>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="news__pagination">
                    <ul class="news__pagination-box">
                        <a href="#" class="news__pagination-item news__pagination-item_active">01</a>
                        <a href="#" class="news__pagination-item">02</a>
                        <a href="#" class="news__pagination-item">03</a>
                        <a href="#" class="news__pagination-item">
                            <svg
                                class="news__pagination-image"
                                width="9"
                                height="16"
                                viewBox="0 0 9 16"
                                fill="none"
                                xmlns="http://www.w3.org/2000/svg"
                            >
                                <path
                                    d="M1.55714 15L7.5 8.31429L1.55714 1.62857"
                                    stroke="#292F36"
                                    stroke-width="2"
                                    stroke-linecap="round"
                                    stroke-linejoin="round"
                                />
                            </svg>
                        </a>
                    </ul>
                </div>
            </div>
        </section>
</template>

<script>
export default {
    name: 'Blog',

    data() {
        return {
            itemsData: [
                { id: 1, src: require('../assets/images/news_photo1.png'), alt: 'news photo', tag: 'Kitchan Design', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022'},
                { id: 2, src: require('../assets/images/news_photo2.png'), alt: 'news photo', tag: 'Living Design',  title: 'Low Cost Latest Invented Interior Designing Ideas.', date: '22 December,2022'},
                { id: 3, src: require('../assets/images/news_photo3.png'), alt: 'news photo', tag: 'Interior Design', title: 'Best For Any Office & Business Interior Solution', date: '25 December,2022'},
                { id: 4, src: require('../assets/images/news_photo4.png'), alt: 'news photo', tag: 'Kitchan Design', title: 'Let’s Get Solution For Building Construction Work', date: '26 December,2022'},
                { id: 5, src: require('../assets/images/news_photo5.png'), alt: 'news photo', tag: 'Living Design', title: 'Low Cost Latest Invented Interior Designing Ideas.', date: '22 December,2022'},
                {id: 6, src: require('../assets/images/news_photo6.png'), alt: 'news photo', tag: 'Interior Design',title: 'Best For Any Office & Business Interior Solution', date: '25 December,2022'}
            ]
        };
    },
};
</script>

<style></style>