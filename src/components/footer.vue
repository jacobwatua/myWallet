<template>
  <div class="footer">

        <div class="top-footer">
            <div v-for="(item, n) in top_footer_items" :key="n">
                <div>
                    <p><strong>{{ item }}</strong></p>
                    <div v-for="(item, n) in footer_options[item]" :key="n" id="links">
                        <p><a href="#" class="text-decoration-none" style="color: white;">{{ item }}</a></p>
                    </div>
                </div>
            </div>
        </div>

        <div class="bottom-footer">
            <div v-for="(item, n) in bottom_footer_items" :key="n">
                <p>{{ item }}</p>
            </div>
        </div>

  </div>
</template>

<script>
export default {
    data () {
        return {
            top_footer_items : ['About Us', 'Contact Us', 'Social Media Links', 'Sitemap', 'Blog'],
            bottom_footer_items : ['Copyright Notice |', 'Terms of Use |', 'Privacy Policy |', 'FAQs |',],
            footer_options : {
                'About Us' : ['Our Story', 'Meet the Team', 'Mission Statement'],
                'Contact Us' : ['Email Us', 'Phone Us', 'Visit Us'],
                'Social Media Links' : ['Facebook', 'Twitter', 'Instagram', 'LinkedIn'],
                'Sitemap' : ['Homepage', 'Categories', 'Tags'],
                'Blog': ['Recent Posts', 'Popular Posts', 'Tags']
            },
        }
    }
}
</script>

<style>
    .footer {
        background-color: black;
        color: white;
        display: grid;
        grid-template-rows: 90% 10%;
        padding: 20px;
        height: 50vh;
    }
    .top-footer{
        display: grid;
        grid-template-columns: repeat(5, 1fr)
    }

    .bottom-footer {
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 10px;
    }
    .bottom-footer p{
        color: orange;
    }
    .links {
        margin-bottom: 20px;
    }
</style>

