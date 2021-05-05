<template>
  
  <div class="flex flex-wrap justify-center items-center bg-white">
    <div class="text-center w-1/2">
      <!-- <h1 class="text-4xl font-bold mt-10"></h1> -->
      <form class="m-2">
        <h1 class="text-2xl font-bold mt-10">Create user on Techines</h1>
        <div class="p-2">
          <div class="mb-4">
            <label class="block text-sm font-bold mb-2 text-left" for="Name">
              Name
            </label>
            <input class="shadow appearance-none border w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="Name" type="text" placeholder="Any">
          </div>
          <div class="mb-4">
            <label class="block text-sm font-bold mb-2 text-left" for="email">
              Email Address
            </label>
            <input class="shadow appearance-none border w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="email" type="text" placeholder="Any">
          </div>
          <div class="mb-4">
            <label class="block text-sm font-bold mb-2 text-left" for="phone">
              Phone Number
            </label>
            <input class="shadow appearance-none border w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="phone" type="text" placeholder="+45 12 34 56 78">
          </div>
          <div class="mb-4">
            <label class="block text-sm font-bold mb-2 text-left" for="password">
              Password
            </label>
            <input class="shadow appearance-none border w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="password" type="text" placeholder="Any">
          </div>
          <div class="mb-4">
            <label class="block text-sm font-bold mb-2 text-left" for="con_password">
              Repate Password
            </label>
            <input class="shadow appearance-none border w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="con_password" type="text" placeholder="any">
          </div>
            <label class="block text-sm mb-2 text-left">Already a user ? <a href="#">Login</a></label>
          <div class="mb-4 mt-4">
            <button class="bg-blue-700 hover:bg-gray-900 text-white py-3 font-bold h-10 inline-flex items-center">
              <svg class="fill-current mt-6" width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M8.1562 0H16.5996V8.39623H16.5524L9.99583 15V6.5566H1.59961L8.1562 0Z" fill="#6CC1FF"/>
              <rect y="6.5" width="10" height="10" fill="white"/>
              </svg>
              <span class="m-3 mr-4">Create user</span>
            </button>
            <!-- <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 w-1/2">Create user</button> -->
          </div>
        </div>
      </form>
    </div>
  </div>
</template>
