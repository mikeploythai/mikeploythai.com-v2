<script lang="ts">
  const navItems = [
    { title: "Projects", path: "#projects" },
    { title: "About", path: "#about" },
    { title: "Resume", path: "/resume", type: "button", target: "_blank" },
  ];
</script>

<nav>
  <div class="container">
    <a href="/" class="size-md brand-md">MP</a>

    <ul>
      {#each navItems as { title, path, type, target } (path)}
        <li>
          <a
            href={path}
            class="size-sm {type}"
            {target}
            rel="noopenner noreferrer"
          >
            {@html title}
          </a>
        </li>
      {/each}
    </ul>
  </div>
</nav>

<style lang="scss">
  nav {
    display: flex;
    position: fixed;
    z-index: 10;
    justify-content: center;
    align-items: center;
    width: 100%;
    padding: 32px 0;
    background-color: var(--navy-blue);

    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 1200px;
      margin: 0 32px;

      ul {
        display: flex;
        gap: 32px;
      }

      a {
        transition: 0.25s ease-in-out;

        &:hover {
          color: var(--highlight-blue);
        }
      }

      .button {
        padding: 8px 12px;
        border: 2px solid var(--baby-blue);
        border-radius: 6px;

        &:hover {
          border: 2px solid var(--highlight-blue);
        }
      }
    }
  }
</style>
