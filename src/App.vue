<template>
  <div id="app" class="antialiased text-gray-900 flex flex-col min-h-screen bg-gray-200">
    <!-- This example requires Tailwind CSS v2.0+ -->
<nav class="bg-blue-50  ">
  <div class="max-w-7xl mx-auto px-2 sm:px-6 lg:px-8">
    <div class="relative flex items-center justify-between h-16">
      <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
        <!-- Mobile menu button-->
        <button type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
          <span class="sr-only">Open main menu</span>
          <!--
            Icon when menu is closed.

            Heroicon name: outline/menu

            Menu open: "hidden", Menu closed: "block"
          -->
          <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
          <!--
            Icon when menu is open.

            Heroicon name: outline/x

            Menu open: "block", Menu closed: "hidden"
          -->
          <svg class="hidden h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>
      <div class="flex-1 flex items-center justify-end sm:items-stretch sm:justify-end">
        
        <div class="hidden sm:block sm:ml-6">
          <div class="flex space-x-4">
            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
            <a href="#" class="text-gray-700 px-3 py-2 rounded-md text-sm font-medium" aria-current="page">About Us</a>

            <a href="#" class="text-gray-700 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Dealer</a>

            <a href="#" class="text-gray-700 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Get Help</a>

            <a href="#" class="text-gray-700 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">News</a>
            <a href="#" class="text-gray-700 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Technies guied  </a>
          </div>
        </div>
      </div>
      <div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">

        <!-- Profile dropdown -->
        <div class="ml-3 relative">
          <div>
            <button type="button" class=" flex text-sm rounded-full focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white" id="user-menu-button" aria-expanded="false" aria-haspopup="true">
              <span class="sr-only">Open user menu</span>
              <img class="h-8 w-8 rounded-full" src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
            </button>
          </div>

          <!--
            Dropdown menu, show/hide based on menu state.

            Entering: "transition ease-out duration-100"
              From: "transform opacity-0 scale-95"
              To: "transform opacity-100 scale-100"
            Leaving: "transition ease-in duration-75"
              From: "transform opacity-100 scale-100"
              To: "transform opacity-0 scale-95"
          -->
          <div class="origin-top-right absolute right-0 mt-2 w-48 rounded-md shadow-lg py-1 bg-white ring-1 ring-black ring-opacity-5 focus:outline-none" role="menu" aria-orientation="vertical" aria-labelledby="user-menu-button" tabindex="-1">
            <!-- Active: "bg-gray-100", Not Active: "" -->
            <a href="#" class="block px-4 py-2 text-sm text-gray-700" role="menuitem" tabindex="-1" id="user-menu-item-0">Your Profile</a>
            <a href="#" class="block px-4 py-2 text-sm text-gray-700" role="menuitem" tabindex="-1" id="user-menu-item-1">Settings</a>
            <a href="#" class="block px-4 py-2 text-sm text-gray-700" role="menuitem" tabindex="-1" id="user-menu-item-2">Sign out</a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Mobile menu, show/hide based on menu state. -->
  <div class="sm:hidden" id="mobile-menu">
    <div class="px-2 pt-2 pb-3 space-y-1">
      <!-- Current: "bg-gray-900 text-white", Default: "text-gray-900 hover:bg-gray-700 hover:text-white" -->
      <a href="#" class="bg-gray-900 text-white block px-3 py-2 rounded-md text-base font-medium" aria-current="page">About Us</a>

      <a href="#" class="text-gray-900 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Dealer</a>

      <a href="#" class="text-gray-900 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Get Help</a>

      <a href="#" class="text-gray-900 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">News</a>
       <a href="#" class="text-gray-900 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Technies guied</a>
    </div>
  </div>
</nav>


    
    <div class="flex items-center justify-between p-4 bg-white logo-header">
      <div class="w-1/5 logo px-10">
          <a href="#">
            <svg width="150" height="50" viewBox="0 0 800 185" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M420.759 32.6829V49.6886H399.236V114.722H381.101V49.6222H359.379V32.6829H420.759Z" fill="#131E35"/>
            <path d="M437.765 116.449C430.325 116.449 424.213 113.925 419.364 108.876C414.515 103.828 412.123 96.7201 412.123 87.6193C412.123 78.4522 414.515 71.4107 419.364 66.3622C424.213 61.3136 430.325 58.7893 437.765 58.7893C445.803 58.7893 451.715 61.845 455.435 67.9565H455.7V60.5165H473.37V114.656H455.7V107.282H455.435C451.715 113.394 445.803 116.449 437.765 116.449ZM442.68 100.241C446.334 100.241 449.39 99.1115 451.715 96.7865C454.04 94.4615 455.235 91.4058 455.235 87.6193C455.235 83.7665 454.04 80.7108 451.715 78.4522C449.39 76.1936 446.334 74.9979 442.68 74.9979C439.093 74.9979 436.104 76.1272 433.779 78.4522C431.454 80.7772 430.258 83.8329 430.258 87.6193C430.258 91.4722 431.454 94.5279 433.779 96.7865C436.104 99.1115 439.093 100.241 442.68 100.241Z" fill="#131E35"/>
            <path d="M510.836 116.449C502.068 116.449 494.893 113.792 489.247 108.478C483.601 103.164 480.744 96.1886 480.744 87.6193C480.744 79.05 483.601 72.075 489.247 66.7607C494.893 61.4465 502.134 58.7893 510.836 58.7893C517.811 58.7893 524.321 60.5165 530.366 64.0372L523.126 78.1865C519.671 75.9943 515.885 74.9315 511.633 74.9315C507.98 74.9315 504.858 76.0608 502.267 78.3193C499.676 80.5779 498.414 83.7 498.414 87.5529C498.414 91.4722 499.676 94.5279 502.267 96.7865C504.858 99.0451 507.98 100.174 511.633 100.174C515.818 100.174 519.671 99.1115 523.126 96.9193L530.366 111.069C524.321 114.656 517.811 116.449 510.836 116.449Z" fill="#131E35"/>
            <path d="M554.347 32.6829V67.6908H554.613C558.532 61.7786 564.311 58.7893 571.951 58.7893C578.195 58.7893 583.177 60.6493 586.831 64.4357C590.484 68.1558 592.344 73.7358 592.344 81.1758V114.656H574.608V86.0915C574.608 78.2529 571.353 74.4 564.776 74.4C557.801 74.4 554.347 78.7843 554.347 87.5529V114.722H536.677V32.6829H554.347Z" fill="#131E35"/>
            <path d="M602.574 114.656V60.5165H620.244V114.656H602.574Z" fill="#131E35"/>
            <path d="M666.279 58.7893C672.523 58.7893 677.506 60.6493 681.159 64.4357C684.813 68.1557 686.673 73.7357 686.673 81.1758V114.656H669.069V86.0915C669.069 78.2529 665.748 74.4 659.105 74.4C652.13 74.4 648.676 78.7843 648.676 87.5529V114.722H631.072V60.5165H648.41V68.6872H648.676C652.528 62.1107 658.441 58.7893 666.279 58.7893Z" fill="#131E35"/>
            <path d="M722.677 58.9221C731.047 58.9221 737.624 61.38 742.34 66.2293C747.123 71.0786 749.514 78.3193 749.514 87.8186V91.8043H710.72C711.783 98.3807 716.433 101.636 724.537 101.636C729.984 101.636 735.232 99.975 740.214 96.72L746.658 110.072C739.816 114.257 732.309 116.383 724.271 116.383C715.237 116.383 707.93 113.792 702.35 108.544C696.836 103.296 694.046 96.3879 694.046 87.8186C694.046 78.8507 696.703 71.7429 701.951 66.6278C707.199 61.5128 714.108 58.9221 722.677 58.9221ZM722.079 71.4107C715.37 71.4107 711.583 74.7321 710.853 81.375H732.376C732.309 78.2529 731.313 75.795 729.386 74.0679C727.46 72.3407 725.002 71.4107 722.079 71.4107Z" fill="#131E35"/>
            <path d="M776.086 116.449C767.251 116.449 759.08 114.589 751.574 110.803L758.283 96.2551C765.391 100.374 771.768 102.433 777.481 102.433C780.736 102.433 782.397 101.636 782.397 99.9751C782.397 99.5765 782.33 99.2443 782.197 98.9122C782.064 98.5801 781.865 98.3143 781.467 98.1815C781.135 97.9822 780.869 97.8493 780.669 97.7165C780.47 97.5836 780.138 97.4508 779.607 97.2515C779.075 97.0522 778.743 96.9193 778.61 96.8529L769.111 93.1329C760.276 89.7451 755.892 84.165 755.892 76.3929C755.892 70.7465 757.818 66.4286 761.737 63.3729C765.657 60.3172 771.436 58.7893 779.075 58.7893C785.32 58.7893 791.829 59.8522 798.605 62.0443L793.69 76.3265C787.18 73.6693 781.865 72.3407 777.614 72.3407C774.691 72.3407 773.296 73.1379 773.296 74.6658C773.296 75.4629 773.628 76.0608 774.226 76.4593C774.824 76.8579 775.887 77.3893 777.415 78.0536L786.781 81.5743C791.165 83.235 794.42 85.2943 796.612 87.7522C798.804 90.2765 799.867 93.6643 799.867 98.0486C799.867 104.293 797.742 108.876 793.557 111.866C789.438 114.922 783.592 116.449 776.086 116.449Z" fill="#131E35"/>
            <path d="M71.6765 184.738H146.741L256.946 74.5994V0H38.3293L0 38.3293V113.062L55.8665 57.1286H127.676V128.938L71.6765 184.738Z" fill="#4D9DE7"/>
            <path d="M55.9993 57.2615H127.742V128.938H127.477L71.6765 184.738V113.062H0L55.9993 57.2615Z" fill="#1350EA"/>
            <path d="M237.682 18.9985V57.1286H165.872V128.938H127.742V57.1286H55.8665V18.9985H237.682Z" fill="white"/>
            <path d="M609.018 32.8822H620.909V44.7065H620.842L611.608 54.0065V42.1158H599.784L609.018 32.8822Z" fill="#0043EC"/></svg>
            </a>
      </div>
      <div class="w-4/5 flex flex-row mr-5 pl-1 btn-logo-header">
          <input class="rounded-none bg-white border-black border-solid border-2 px-5 font-bold w-3/5 h-12 width-full-mobile" placeholder="What are you looking for ?" />
          <button class="bg-gray-800 text-xs hover:bg-gray-900 text-white py-3 font-bold h-12 -ml-2 mr-4 inline-flex items-center">
              <svg class="fill-current mt-8"  width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M8.1562 0H16.5996V8.39623H16.5524L9.99583 15V6.5566H1.59961L8.1562 0Z" fill="#CBD0DA"/>
              <rect y="6.5" width="10" height="10" fill="white"/>
              </svg>
              <span class="m-3 mr-4">Search</span>
            </button>

            <button class="bg-blue-300 text-xs hover:bg-gray-900 text-white py-1 font-bold h-12 -ml-2 mr-4 inline-flex items-center display-mobile-view">
              <svg class="fill-current mt-8"  width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M8.1562 0H16.5996V8.39623H16.5524L9.99583 15V6.5566H1.59961L8.1562 0Z" fill="#043ED6"/>
              <rect y="6.5" width="10" height="10" fill="white"/>
              </svg>
              <span class="m-3 mr-4">Become Dealer</span>
            </button>

            <button class="bg-blue-900 text-xs hover:bg-gray-900 text-white py-3 font-bold h-12 -ml-2 inline-flex items-center display-mobile-view">
              <svg class="fill-current mt-8" width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M8.1562 0H16.5996V8.39623H16.5524L9.99583 15V6.5566H1.59961L8.1562 0Z" fill="#6CC1FF"/>
              <rect y="6.5" width="10" height="10" fill="white"/>
              </svg>
              <span class="m-3 mr-4">Create Advertisement</span>
            </button>
          </div>
      </div>

    <div class="p-2 middle-part-main">
      <div class="flex flex-row p-3">
        <div class="m-3 w-1/6">
            <div class="bg-blue-100 h-48 m-2 rounded"></div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
        </div>
        <div class="m-3 w-3/5">
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
            <div class="m-5 p-5">
              <router-view class="flex-1"/>
            </div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
        
        </div>
        <div class="m-3 w-1/6">
            <div class="bg-blue-100 h-48 m-2 rounded"></div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
            <div class="bg-blue-100 h-24 m-2 rounded"></div>
        
        </div>
      </div>
    </div>
    
    <div class="flex flex-row p-4 footer-part" style="background:#131E35">
      <div class="w-3/5 flex flex-row pl-8 pt-8">
        <div class="w-1/5 ">
        </div>
        <div class="w-1/5">
          <p class="text-1xl font-bold text-white">Footer 1</p>
          <ul class="text-sm text-white pt-5">
            <li>Service 1</li>
            <li>Service 2</li>
            <li>Service 3</li>
            <li>Service 4</li>
          </ul>
        </div>
        <div class="w-1/5 ">
          <p class="text-1xl font-bold text-white">Footer 2</p>
            <ul class="text-sm text-white pt-5">
              <li>Product 1</li>
              <li>Product 2</li>
              <li>Product 3</li>
              <li>Product 4</li>
            </ul>
        </div>
        <div class="w-1/5 ">
          <p class="text-1xl font-bold text-white">Footer 3</p>
          <ul class="text-sm text-white pt-5">
              <li>Footer item 1</li>
              <li>Footer item 2</li>
              <li>Footer item 3</li>
              <li>Footer item 4</li>
          </ul>
        </div>
        <div class="w-1/5 divide-x divide-green-500">
          <p class="text-1xl font-bold text-white">Footer 4</p>
          <ul class="text-sm text-white pt-5">
              <li>Footer item 1</li>
              <li>Footer item 2</li>
              <li>Footer item 3</li>
              <li>Footer item 4</li>
          </ul>
        </div>
      </div>
      <div class="bg-white border-r-2"></div>
      <div class="w-2/5 pt-4 pl-5">
        <div class="flex-shrink-1">
            <svg width="150" height="50" viewBox="0 0 217 50" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M113.751 8.8457V13.4482H107.933V31.0491H103.03V13.4302H97.1572V8.8457H113.751Z" fill="white"/>
              <path d="M118.349 31.518C116.338 31.518 114.685 30.8347 113.374 29.4683C112.064 28.1018 111.417 26.178 111.417 23.7148C111.417 21.2336 112.064 19.3278 113.374 17.9613C114.685 16.5948 116.338 15.9116 118.349 15.9116C120.522 15.9116 122.12 16.7387 123.126 18.3928H123.198V16.3791H127.975V31.0325H123.198V29.0368H123.126C122.12 30.6909 120.522 31.518 118.349 31.518ZM119.678 27.1309C120.666 27.1309 121.492 26.8253 122.12 26.196C122.749 25.5667 123.072 24.7396 123.072 23.7148C123.072 22.672 122.749 21.8449 122.12 21.2336C121.492 20.6223 120.666 20.2987 119.678 20.2987C118.708 20.2987 117.9 20.6043 117.272 21.2336C116.643 21.8629 116.32 22.69 116.32 23.7148C116.32 24.7576 116.643 25.5847 117.272 26.196C117.9 26.8253 118.708 27.1309 119.678 27.1309Z" fill="white"/>
              <path d="M138.103 31.518C135.733 31.518 133.793 30.7988 132.267 29.3604C130.74 27.922 129.968 26.0342 129.968 23.7148C129.968 21.3954 130.74 19.5076 132.267 18.0692C133.793 16.6308 135.751 15.9116 138.103 15.9116C139.989 15.9116 141.749 16.3791 143.383 17.332L141.426 21.1617C140.492 20.5684 139.468 20.2807 138.319 20.2807C137.331 20.2807 136.487 20.5863 135.786 21.1976C135.086 21.8089 134.745 22.654 134.745 23.6968C134.745 24.7576 135.086 25.5847 135.786 26.196C136.487 26.8073 137.331 27.1129 138.319 27.1129C139.45 27.1129 140.492 26.8253 141.426 26.2319L143.383 30.0616C141.749 31.0325 139.989 31.518 138.103 31.518Z" fill="white"/>
              <path d="M149.867 8.8457V18.3208H149.939C150.998 16.7206 152.561 15.9115 154.626 15.9115C156.314 15.9115 157.661 16.415 158.649 17.4398C159.636 18.4466 160.139 19.9569 160.139 21.9705V31.0321H155.344V23.301C155.344 21.1795 154.464 20.1367 152.686 20.1367C150.801 20.1367 149.867 21.3233 149.867 23.6965V31.05H145.09V8.8457H149.867Z" fill="white"/>
              <path d="M162.904 31.0317V16.3804H167.681V31.0317H162.904Z" fill="white"/>
              <path d="M180.128 15.9116C181.816 15.9116 183.163 16.415 184.15 17.4398C185.138 18.4466 185.641 19.9568 185.641 21.9705V31.0318H180.882V23.3009C180.882 21.1794 179.984 20.1366 178.188 20.1366C176.302 20.1366 175.368 21.3232 175.368 23.6964V31.0497H170.609V16.3791H175.297V18.5905H175.368C176.41 16.8106 178.008 15.9116 180.128 15.9116Z" fill="white"/>
              <path d="M195.374 15.9478C197.637 15.9478 199.415 16.613 200.69 17.9256C201.983 19.2381 202.629 21.1979 202.629 23.7691V24.8479H192.141C192.429 26.6279 193.686 27.5089 195.877 27.5089C197.349 27.5089 198.768 27.0594 200.115 26.1784L201.857 29.7923C200.007 30.9251 197.978 31.5004 195.805 31.5004C193.363 31.5004 191.387 30.7992 189.879 29.3788C188.388 27.9584 187.634 26.0885 187.634 23.7691C187.634 21.3418 188.352 19.4179 189.771 18.0334C191.19 16.649 193.057 15.9478 195.374 15.9478ZM195.212 19.328C193.399 19.328 192.375 20.227 192.177 22.025H197.996C197.978 21.1799 197.709 20.5147 197.188 20.0472C196.667 19.5797 196.003 19.328 195.212 19.328Z" fill="white"/>
              <path d="M209.813 31.518C207.425 31.518 205.216 31.0145 203.187 29.9897L205 26.0521C206.922 27.1669 208.646 27.7243 210.19 27.7243C211.07 27.7243 211.519 27.5085 211.519 27.059C211.519 26.9511 211.501 26.8612 211.466 26.7713C211.43 26.6814 211.376 26.6095 211.268 26.5736C211.178 26.5196 211.106 26.4837 211.052 26.4477C210.999 26.4117 210.909 26.3758 210.765 26.3218C210.621 26.2679 210.532 26.2319 210.496 26.214L207.928 25.2071C205.539 24.2901 204.354 22.7799 204.354 20.6762C204.354 19.148 204.875 17.9793 205.934 17.1522C206.994 16.3252 208.556 15.9116 210.621 15.9116C212.31 15.9116 214.07 16.1993 215.901 16.7926L214.572 20.6583C212.812 19.9391 211.376 19.5795 210.226 19.5795C209.436 19.5795 209.059 19.7952 209.059 20.2088C209.059 20.4245 209.149 20.5863 209.31 20.6942C209.472 20.8021 209.759 20.9459 210.173 21.1257L212.705 22.0786C213.89 22.5281 214.77 23.0855 215.363 23.7508C215.955 24.434 216.243 25.3509 216.243 26.5376C216.243 28.2277 215.668 29.4683 214.537 30.2774C213.423 31.1044 211.843 31.518 209.813 31.518Z" fill="white"/>
              <path d="M19.3775 50H39.671L69.4646 20.1906V0H10.3622L0 10.374V30.6005L15.1034 15.4621H34.5168V34.8975L19.3775 50Z" fill="#6CC1FF"/>
              <path d="M15.1393 15.4983H34.5348V34.8978H34.4629L19.3775 50.0002V30.6007H0L15.1393 15.4983Z" fill="url(#paint0_linear)"/>
              <path d="M64.2567 5.14185V15.4618H44.8433V34.8972H34.5349V15.4618H15.1035V5.14185H64.2567Z" fill="white"/>
              <path d="M164.647 8.89941H167.861V12.1001H167.843L165.347 14.6175V11.3988H162.15L164.647 8.89941Z" fill="white"/>
              <defs>
              <linearGradient id="paint0_linear" x1="17.2674" y1="15.4983" x2="17.2674" y2="50.0002" gradientUnits="userSpaceOnUse">
              <stop stop-color="#043ED6"/>
              <stop offset="1" stop-color="#002B9D"/>
              </linearGradient>
              </defs>
            </svg>

            <p class="text-1xl text-xs text-white mt-5">You are always welcome to contact us by e-mail.</p>
            <p class="text-1xl font-bold text-xs text-white mt-5">hello@tachines.com</p>
            <div class="flex flex-row pt-4">
              <div class="pr-8 pt-4">
                <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M16 32C24.8366 32 32 24.8366 32 16C32 7.16344 24.8366 0 16 0C7.16344 0 0 7.16344 0 16C0 24.8366 7.16344 32 16 32Z" fill="white"/>
                <path d="M17.6656 12.3274H18.5785V10.7374C18.421 10.7157 17.8794 10.667 17.2485 10.667C15.9323 10.667 15.0306 11.4949 15.0306 13.0166V14.417H13.5781V16.1945H15.0306V20.667H16.8115V16.1949H18.2052L18.4265 14.4174H16.811V13.1928C16.8115 12.6791 16.9498 12.3274 17.6656 12.3274Z" fill="#043ED6"/>
                </svg>
              </div>
              <div class="pl-4 pr-8 pt-4">
                <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M16 32C24.8366 32 32 24.8366 32 16C32 7.16344 24.8366 0 16 0C7.16344 0 0 7.16344 0 16C0 24.8366 7.16344 32 16 32Z" fill="white"/>
                <path fill-rule="evenodd" clip-rule="evenodd" d="M16 24C20.4183 24 24 20.4183 24 16C24 11.5817 20.4183 8 16 8C11.5817 8 8 11.5817 8 16C8 20.4183 11.5817 24 16 24Z" fill="#043ED6"/>
                <path d="M24.5576 6H7.44241C6.64575 6 6 6.65739 6 7.4684V24.8919C6 25.703 6.64575 26.3604 7.44241 26.3604H24.5576C25.3542 26.3604 26 25.703 26 24.8919V7.4684C26 6.65739 25.3542 6 24.5576 6V6ZM13.0941 21.3896H10.6587V13.9304H13.0941V21.3896ZM11.8765 12.9119H11.8606C11.0433 12.9119 10.5148 12.3392 10.5148 11.6234C10.5148 10.8914 11.0595 10.3345 11.8926 10.3345C12.7258 10.3345 13.2385 10.8914 13.2543 11.6234C13.2543 12.3392 12.7258 12.9119 11.8765 12.9119ZM21.8759 21.3896H19.4407V17.3991C19.4407 16.3962 19.0881 15.7123 18.2069 15.7123C17.5341 15.7123 17.1334 16.1737 16.9573 16.619C16.8929 16.7784 16.8772 17.0011 16.8772 17.224V21.3896H14.4419C14.4419 21.3896 14.4738 14.6302 14.4419 13.9304H16.8772V14.9866C17.2009 14.4783 17.7799 13.7554 19.0721 13.7554C20.6744 13.7554 21.8759 14.8214 21.8759 17.1125V21.3896Z" fill="white"/>
                </svg>

              </div>
              <div class="pl-4 pr-8 pt-4">
                <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M16 32C24.8366 32 32 24.8366 32 16C32 7.16344 24.8366 0 16 0C7.16344 0 0 7.16344 0 16C0 24.8366 7.16344 32 16 32Z" fill="white"/>
                <path d="M20.667 12.6289C20.2951 12.792 19.8989 12.9001 19.4857 12.9526C19.9107 12.6989 20.2351 12.3001 20.3876 11.8195C19.9914 12.0557 19.5539 12.2226 19.0876 12.3157C18.7114 11.9151 18.1751 11.667 17.5901 11.667C16.4551 11.667 15.5414 12.5882 15.5414 13.7176C15.5414 13.8801 15.5551 14.0364 15.5889 14.1851C13.8845 14.102 12.3764 13.2851 11.3632 12.0407C11.1864 12.3476 11.0826 12.6989 11.0826 13.077C11.0826 13.787 11.4482 14.4164 11.9932 14.7807C11.6639 14.7745 11.3407 14.6789 11.067 14.5282C11.067 14.5345 11.067 14.5426 11.067 14.5507C11.067 15.547 11.7776 16.3745 12.7095 16.5651C12.5426 16.6107 12.3607 16.6326 12.172 16.6326C12.0407 16.6326 11.9082 16.6251 11.7839 16.5976C12.0495 17.4095 12.8032 18.0064 13.6995 18.0257C13.002 18.5714 12.1164 18.9001 11.1576 18.9001C10.9895 18.9001 10.8282 18.8926 10.667 18.872C11.5751 19.4576 12.6514 19.792 13.812 19.792C17.5845 19.792 19.647 16.667 19.647 13.9582C19.647 13.8676 19.6439 13.7801 19.6395 13.6932C20.0464 13.4045 20.3882 13.0439 20.667 12.6289Z" fill="#043ED6"/>
                </svg>

              </div>
              <div class="pl-4 w-1/4 pt-4">
                <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M16 32C24.8365 32 32 24.8366 32 16C32 7.16344 24.8365 0 16 0C7.16344 0 0 7.16344 0 16C0 24.8366 7.16344 32 16 32Z" fill="white"/>
                <path d="M18.208 10.667H14.458C12.7324 10.667 11.333 12.0664 11.333 13.792V17.542C11.333 19.2676 12.7324 20.667 14.458 20.667H18.208C19.9336 20.667 21.333 19.2676 21.333 17.542V13.792C21.333 12.0664 19.9336 10.667 18.208 10.667ZM20.3955 17.542C20.3955 18.7482 19.4143 19.7295 18.208 19.7295H14.458C13.2518 19.7295 12.2705 18.7482 12.2705 17.542V13.792C12.2705 12.5857 13.2518 11.6045 14.458 11.6045H18.208C19.4143 11.6045 20.3955 12.5857 20.3955 13.792V17.542Z" fill="#043ED6"/>
                <path d="M16.333 13.167C14.9524 13.167 13.833 14.2864 13.833 15.667C13.833 17.0476 14.9524 18.167 16.333 18.167C17.7136 18.167 18.833 17.0476 18.833 15.667C18.833 14.2864 17.7136 13.167 16.333 13.167ZM16.333 17.2295C15.4718 17.2295 14.7705 16.5282 14.7705 15.667C14.7705 14.8051 15.4718 14.1045 16.333 14.1045C17.1943 14.1045 17.8955 14.8051 17.8955 15.667C17.8955 16.5282 17.1943 17.2295 16.333 17.2295Z" fill="#043ED6"/>
                <path d="M19.0206 13.3127C19.2046 13.3127 19.3538 13.1636 19.3538 12.9796C19.3538 12.7956 19.2046 12.6465 19.0206 12.6465C18.8366 12.6465 18.6875 12.7956 18.6875 12.9796C18.6875 13.1636 18.8366 13.3127 19.0206 13.3127Z" fill="#043ED6"/>
                </svg>

              </div>
            </div>

        </div>
      </div>
    </div>
    <div class="flex flex-row p-4 footer-part" style="background:#131E35">

      <div class="w-1/6 "></div>
      <div class="w-full border-t-2">
        <div class="flex flex-row">
          <div class="w-1/2 mt-5">
            <p class="text-white text-xs font-bold">Copyright © 2020 Tachines | all right reserved</p>
          </div>
          <div class="w-1/2 mt-5">
          <ul class="flex flex-row-reverse">
            <li class="text-white text-xs font-bold float-right ml-10">Cookie policy</li>
            <li class="text-white text-xs font-bold float-right">Terms & conditions</li>
          </ul>
          </div>
        </div>
      </div>
      <div class="w-1/6 "></div>
    </div>

  </div>
</template>

<style>
@tailwind base;
@tailwind components;
@font-face {
  font-family: 'GTEestiProDisplay-Regular';
  src: local('GTEestiProDisplay-Regular'), url(/assets/fonts/GTEestiProDisplay-Regular.ttf) format('ttf');
}
@tailwind utilities;
.origin-top-right {
  transform-origin: top right;
}
.transition-all {
  transition-property: all;
}
.transition-fastest {
  transition-duration: 50ms;
}
.transition-faster {
  transition-duration: 100ms;
}
.transition-fast {
  transition-duration: 150ms;
}
.transition-medium {
  transition-duration: 200ms;
}
.ease-out-quad {
  transition-timing-function: cubic-bezier(.25, .46, .45, .94);
}
.ease-in-quad {
  transition-timing-function: cubic-bezier(.55, .085, .68, .53);
}
.scale-70 {
  transform: scale(.7);
}
.scale-100 {
  transform: scale(1);
}


@media (max-width: 640px) {
  
}

@media (max-width: 768px) {
  .middle-part-main .w-3\/5 {
      width: 100%;
  }
  .middle-part-main .w-1\/2 {
    width: 80%;
  }
  .middle-part-main .h-24 {
    height: auto;
}
.middle-part-main .w-1\/6 {
    width: auto;
    margin: 0px;
    padding: 0px;
    display: none;
}
.middle-part-main .w-3\/5 .m-5.p-5 {
  padding: 0px;
  margin: 0px;
}
.logo-header {
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.logo-header .width-full-mobile {
    width: 100%;
    justify-content: center;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.logo-header .w-3\/5 {
    width: 100%;
    margin: 0px 0px 10px;
}
.btn-logo-header {
    display: block;
    width: 100%;
}
.logo-header button {
  margin: 0px 0px 15px !important;
  width: 100%;

}
.footer-part {
    display: block;
}
.footer-part .w-3\/5 {
    width: 100%;
    padding: 0px;
}
.footer-part .w-3\/5 {
    width: 100%;
    padding: 0px;
    DISPLAY: BLOCK;
}
.footer-part .w-2\/5 {
    width: 100%;
    PADDING: 20px 0px;
}
}

@media (max-width: 1280px) {
  .middle-part-main .w-3\/5 {
      width: 100%;
  }
  .middle-part-main .w-1\/2 {
    width: 80%;
  }
  .middle-part-main .h-24 {
    height: auto;
}
.middle-part-main  .mr-20 {
    margin-right: 2rem;
}
.logo-header .w-1\/5 {
    width: 34%;
    padding: 0px;
}
}





</style>
