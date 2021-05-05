<template>
  <header>
      <div class="container">
          <a href="#">
              <img class="brand" src="../assets/img/dc-logo.png" alt="logo DC">
          </a>
            <nav>
                <ul>
                    <li>
                        <a href="#">characters</a>
                    </li>
                    <li>
                        <a href="#">comics</a>
                    </li>
                    <li>
                        <a href="#">movies</a>
                    </li>
                    <li>
                        <a href="#">tv</a>
                    </li>
                    <li>
                        <a href="#">games</a>
                    </li>
                    <li>
                        <a href="#">collectibles</a>
                    </li>
                    <li>
                        <a href="#">videos</a>
                    </li>
                    <li>
                        <a href="#">fans</a>
                    </li>
                    <li>
                        <a href="#">news</a>
                    </li>
                    <li>
                        <a href="#">shop</a>
                    </li>
                </ul>
            </nav>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style lang="scss" scoped>
    header {
        font-weight: 600;
        text-transform: uppercase;
    }
    .container {
        display: flex;
        height: 120px;
        justify-content: space-between;
        align-items: center;
        .brand {
            height: 80px;
        }
        li {
            display:inline-flex;
            &:not(:last-of-type) {
                margin-right: 1.8rem;
            }
        }
    }
</style>