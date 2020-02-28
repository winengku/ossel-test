<template>
    <div class="row mx-0 navbar-container align-items-center">
        <div class="col-5 mx-0">
            PRODUCT CATEGORIES <i class="ml-5 fa fa-caret-down"></i>
        </div>
        <div class="col-7 mx-0 px-0">
            <nav class="navbar navbar-expand-lg">
                <ul class="navbar-nav">
                    <li v-for="routes in links" :key="routes.id" class="nav-item mr-80"><a href=#> {{routes.text}} </a></li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Navigation',
  data() {
    return {
      links: [
        {
          id: 0,
          text: 'BEST SELLER',
          page:'#'
        },
        {
          id: 1,
          text: 'ABOUT US',
          page:'#'
        },
        {
          id: 2,
          text: 'CONTACT',
          page:'#'
        }
      ]
    }
  }
}
</script>