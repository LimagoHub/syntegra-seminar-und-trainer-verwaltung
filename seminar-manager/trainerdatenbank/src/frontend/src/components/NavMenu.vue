<template>
    <header>
      <nav class="navbar navbar-expand-md bg-dark navbar-dark">
        <!-- Brand -->
        <a class="navbar-brand" href="#">Syntegrata</a>

        <!-- Toggler/collapsibe Button -->
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Navbar links -->
        <div class="collapse navbar-collapse" id="collapsibleNavbar">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link :to="{ name: 'HelloWorld' }" class="nav-link">Home</router-link>

            </li>
            <li class="nav-item">
              <router-link :to="{ name: 'MyTest' }" class="nav-link">Trainer</router-link>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Skills</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
          </ul>
        </div>
      </nav>

    </header>
</template>




<style>
a.navbar-brand {
    white-space: normal;
    text-align: center;
    word-break: break-all;
}

html {
    font-size: 14px;
}

@media (min-width: 768px) {
    html {
        font-size: 16px;
    }
}

.box-shadow {
    box-shadow: 0 .25rem .75rem rgba(0, 0, 0, .05);
}
</style>

<script>
export default {
    name: 'NavMenu',
    data() {
        return {
            isExpanded: false
        }
    },
    methods: {
        collapse() {
            this.isExpanded = false;
        },

        toggle() {
            this.isExpanded = !this.isExpanded;
        }
    }
}
</script>
