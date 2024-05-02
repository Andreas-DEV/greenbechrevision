<script>
  import {
    Navbar,
    NavBrand,
    NavLi,
    NavUl,
    NavHamburger,
    Dropdown,
    DropdownItem,
    DropdownDivider,
  } from "flowbite-svelte";
  import { ChevronDownOutline } from "flowbite-svelte-icons";
  import { page } from "$app/stores";
  $: activeUrl = $page.url.pathname;

  import logoSort from "$lib/assets/Greenbech-Revision-Sort.png";
  import logoHvid from "$lib/assets/Greenbech-Revision-Hvid.png";
  import NavContainer from "flowbite-svelte/NavContainer.svelte";
</script>

<Navbar>
  <NavContainer class="flex justify-around">
    <NavBrand href="/">
      <img src={logoSort} class="w-[125px]" alt="Grønbech Revision Logo" />
    </NavBrand>
    <NavHamburger />
    <NavUl {activeUrl}>
      <NavLi href="/">Hjem</NavLi>
      <NavLi class="cursor-pointer" href="/bogforing-regnskab">
        Bogføring & regnskab<ChevronDownOutline
          class="w-6 h-6 ms-2 text-primary-800 dark:text-white inline"
        />
      </NavLi>
      <Dropdown trigger="hover" class="w-44 z-20">
        <DropdownItem href="/lon-administration">Lønadministration</DropdownItem
        >
      </Dropdown>
      <NavLi href="/om-os">Om os</NavLi>
      <NavLi href="/kontakt">Kontakt</NavLi>
    </NavUl>
  </NavContainer>
</Navbar>
