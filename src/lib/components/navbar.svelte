<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte'
  import Logo from './CuatexLogo.svg';
</script>

<Navbar let:hidden let:toggle>
    <NavBrand href="/">
      <img
        src={Logo}
        class="mr-3 h-6 sm:h-14"
        alt="Cuatex Logo"
      />
    </NavBrand>
    <NavHamburger on:click={toggle} />
    <NavUl {hidden}>
      <NavLi href="/creators">
        <div class="text-orange-500">
            Creators
        </div>
      </NavLi>
      <NavLi href="/careers">
        <div class="text-orange-500">
            Careers
        </div>
      </NavLi>
      <NavLi href="/investors">
        <div class="text-orange-500">
            Investors            
        </div>
    </NavLi>
      <NavLi href="/about-us">
        <div class="text-orange-500">       
            About Us
        </div>
       </NavLi>
    </NavUl>
  </Navbar>  