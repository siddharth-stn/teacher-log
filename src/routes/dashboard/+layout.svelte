<script>
  export let staff_name = "staff_name";
</script>

<div>
  <!-- body wrapper -->
  <div class="p-2 border border-b-blue-600 flex">
    <!-- menu wrapper -->
    <div class="">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        fill="currentColor"
        class="w-6 h-6"
      >
        <path
          fill-rule="evenodd"
          d="M3 6.75A.75.75 0 013.75 6h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 6.75zM3 12a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 12zm0 5.25a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75a.75.75 0 01-.75-.75z"
          clip-rule="evenodd"
        />
      </svg>
    </div>
    <div class="flex-1 text-center">
      <span class="font-semibold">Dashboard</span>
    </div>
    <div class="w-6 h-6" />
  </div>
  <div class="p-4">
    <!-- main wrapper -->
    <div class="text-right">
      <span>Hello, {staff_name}</span>
    </div>
    <div class=" flex flex-col gap-4 mt-4">
      <!-- previous logs data -->
      <span class="self-center">Previous Logs</span>
      <div class="">
        <table class="min-w-full">
          <tr><th colspan="3" class="text-red-600">Incomplete</th></tr>
          <tr>
            <th class="">Date</th>
            <th class="">Remarks</th>
            <th class="">Action</th>
          </tr>
        </table>
      </div>
      <div>
        <!-- complete logs table -->
        <table class="min-w-full">
          <tr><th colspan="3" class="text-green-600">Complete</th></tr>
          <tr>
            <th class="">Date</th>
            <th class="">Remarks</th>
            <th class="">Action</th>
          </tr>
        </table>
      </div>
    </div>
    <div class="mt-6">
      <!-- form to get data to see log for a particular route -->
      <form action="" class="flex gap-1">
        <input
          type="date"
          class="grow border border-blue-500 px-3 py-2 rounded-md focus:outline-none focus:border-orange-400 hover:border-orange-400"
        />
        <button
          type="submit"
          class="grow-0 border border-blue-500 rounded-md px-3 py-2 bg-blue-400 text-white"
          >See Log</button
        >
      </form>
    </div>
    <div class="mt-6 flex">
      <!-- Goto log entry page -->
      <button
        class="grow border border-blue-500 rounded-md px-3 py-2 bg-blue-400 text-white"
        >Enter today's Log</button
      >
    </div>
  </div>
</div>

<slot />

<style>
  table,
  th,
  td {
    border: 1px solid black;
    border-collapse: collapse;
  }
</style>
