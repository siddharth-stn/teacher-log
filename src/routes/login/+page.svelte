<div class="h-screen flex items-center">
  <form class="w-11/12 mx-auto">
    <div class="border-solid border-2 border-red-500 flex flex-col gap-4">
      <div class="flex flex-col mx-auto">
        <label for="admin"><input type="radio" id="admin" />Admin</label>
        <label for="employee"
          ><input type="radio" id="employee" />Employee</label
        >
      </div>

      <div class="flex flex-col">
        <label for="email">
          <input type="email" placeholder="Enter your email..." /></label
        >
        <label for="password">
          <input type="password" placeholder="Enter password..." /></label
        >
      </div>

      <div>
        <button type="submit">login</button>
      </div>
    </div>
  </form>
</div>
