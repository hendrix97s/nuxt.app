<template>
<div class="flex flex-col w-full p-4">
  <div class="overflow-x-auto">
    <div class="rounded-lg">
      <div class="overflow-hidden rounded-lg shadow-2xl">
        <table class="w-full text-center">
          <thead class="border-b bg-gray-800">
            <tr>
              <th scope="col" class="text-sm font-medium text-white px-6 py-4">
                #
              </th>
              <th scope="col" class="text-sm font-medium text-white px-6 py-4">
                First
              </th>
              <th scope="col" class="text-sm font-medium text-white px-6 py-4">
                Last
              </th>
              <th scope="col" class="text-sm font-medium text-white px-6 py-4">
                Handle
              </th>
            </tr>
          </thead>
          <tbody>
            <tr class="bg-white border-b" v-for="index in 10" :key="index">
              <td class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900">1</td>
              <td class="text-sm text-gray-900 font-light px-6 py-4 whitespace-nowrap">
              </td>
              <td class="text-sm text-gray-900 font-light px-6 py-4 whitespace-nowrap">
                Otto
              </td>
              <td class="text-sm text-gray-900 font-light px-6 py-4 whitespace-nowrap">
                @mdo
              </td>
            </tr>
            
          </tbody>            
         </table>
      </div>
    </div>
  </div>
</div>
</template>
  
<script>
export default {
  name: 'Schedule',
  el: '#example-1',
  data: {
    items: [
      { message: 'Algo' },
      { message: 'Outro' }
    ]
  }
}
</script>