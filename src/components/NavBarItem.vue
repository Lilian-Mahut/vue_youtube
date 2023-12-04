<template>
  <div id="left-container">
    <div id="burger">
      <slot name="burger" id="logo"></slot>
    </div>
    <div id="logo">
      <a href="/" title="Accueil YouTube">
        <slot name="logo" id="ytlogo"></slot>
      </a>
      <div id="location">
        <span id="country-code">
          FR
        </span>
      </div>
    </div>
  </div>
  <div class="center-container">
    <slot name="search">
      <form id="search-form">
        <div class="container">
          <div id="container">
            <div id="search-input">
              <input
                id="search"
                autocapitalize="none"
                autocomplete="off"
                autocorrect="off"
                name="search_query"
                tabindex="0" type="text"
                spellcheck="false"
                placeholder="Rechercher"
                aria-label="Rechercher"
                role="combobox"
                aria-haspopup="false"
                aria-autocomplete="list"
                dir="ltr" style="outline: none;"
                class="ytd-searchbox">
            </div>
          </div>
        </div>
      </form>
      <button id="search-icon" aria-label="Rechercher">
        <slot name="search-icon"></slot>
      </button>
    </slot>
  </div>
  <div class="right-container">
    <slot name="user"></slot>
  </div>
</template>

<style scoped>
template {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
#left-container {
  display: flex;
  justify-content: center;
}
#burger {
  margin-left: 1rem;
}
#logo {
  display: flex;
  align-items: center;
}
#search-form {
  height: 40px;
  position: relative;
  -moz-box-flex: 1;
  flex: 1;
  display: flex;
  flex-direction: row;
}
#container {
  position: relative;
  -moz-box-align: center;
  align-items: center;
  background-color: transparent;
  border: 1px solid #303030;
  border-radius: 40px 0 0 40px;
  box-shadow: inset 0 1px 2px #0d0d0d;
  padding: 0 4px 0 16px;
  margin-left: 32px;
  flex: 1;
  display: flex;
  flex-direction: row;
}
.search-input {
  width: 100%;
}
#search {
  outline: none;
}

@media (min-width: 1024px) {
  .logo {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .logo:before {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    bottom: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .logo:after {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    top: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .logo:first-of-type:before {
    display: none;
  }

  .item:last-of-type:after {
    display: none;
  }
}
</style>
