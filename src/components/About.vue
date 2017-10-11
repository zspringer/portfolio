<template>
    <div id="about-me">
        <h2>{{msg}}</h2>
        <section>
            <v-layout>
                <v-flex xs12 sm6 offset-sm3>
                    <v-card>
                        <v-card-media src="https://res.cloudinary.com/dmyvekzok/image/upload/v1507594278/IMG_2289_tp395i.jpg" height="600px">
                        </v-card-media>
                        <v-card-title primary-title>
                            <div>
                                <h3 class="headline mb-0">About Me</h3>
                                <!-- <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div> -->
                                <div>
                                    <p>Hello. I want to start off by stating a huge "THANK YOU" for visiting my website. I grew
                                        up in Anaheim, CA and moved to Boise, ID in high school. After high school, I attended
                                        Boise State University and obtained a B.S. degree in Business Administration. During
                                        college, I worked for an attorney for several years before working for the Federal
                                        Court system. I am married with four awesome children. My wife,
                                        <a class="julie" href="http://www.empoweragilecoaching.com">
                                            <strong>Julie Springer</strong>
                                        </a>, is Agile and Leadership coach.</p>
                                    <p>I've always been interested in development work and decided to make a career change after
                                        14 years with the government. I'm so excited to work in this field where I can converge
                                        my passion and enthusiasm to create awesome products that are functional and possess
                                        that "wow" factor. I have a strong belief in creating products that really work for
                                        the end-user. I'm extremely client and team oriented and I want to make the best product that
                                        is easily maintainable and most importantly, WORKS the way you want it to.</p>
                                    </p>
                                </div>
                            </div>
                        </v-card-title>
                        <!-- <v-card-actions>
                              <v-btn flat color="orange">Share</v-btn>
                              <v-btn flat color="orange">Explore</v-btn>
                            </v-card-actions> -->
                    </v-card>
                </v-flex>
            </v-layout>
            <!-- <v-parallax src="assets/section.jpeg" height="380">
                <v-layout column align-center justify-center>
                    <div class="headline white--text mb-3">Web development has never been easier</div>
                    <em>Kick-start your application today</em>
                    <v-btn class="blue lighten-2 mt-5" dark large href="/pre-made-themes">
                        Get Started
                    </v-btn>
                </v-layout>
            </v-parallax> -->
        </section>
    </div>
</template>

<script>
    export default {
        name: 'about',
        data() {
            return {
                msg: 'About Me'
            }
        }

    }
</script>

<style scoped>
    #about-me {
        padding-top: 100px;
        padding-bottom: 100px;
    }
</style>