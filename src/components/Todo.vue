<template>
  <div class="container mx-auto mt-2.5">
    <div class="border border-[#E0E3EB] rounded-md overflow-hidden">
      <div class="py-4 px-5 flex items-center bg-[#F7F8FC]">
        <div class="basis-[70%] flex items-center">
          <div class="font-semibold text-sm text-[#42A5F5]">
            {{ todoList.date }}
          </div>
          <div v-if="!todoList.time" class="ml-2.5 flex items-center gap-x-5">
            <div class="font-semibold text-[#12192F]">00:00:00</div>
            <div class="font-semibold text-sm text-[#12192F]">0,00$</div>
          </div>
        </div>
        <div
          class="font-semibold text-[#12192F] basis-[10%]"
          v-if="todoList.time"
        >
          {{ todoList.time }}
        </div>
        <div
          class="font-semibold text-[#12192F] basis-[10%] ml-5"
          v-if="todoList.price"
        >
          {{ todoList.price }}
        </div>
        <div
          class="ml-auto flex items-center gap-x-2.5 cursor-pointer"
          @click="
            () => {
              setIsOpen(!isOpen);
            }
          "
        >
          <div class="text-xs text-[#686D7B]">Свернуть</div>
          <ChevronDown />
        </div>
      </div>
      <div class="bg-white" v-show="isOpen">
        <div
          :class="[
            'py-2.5 px-5 border-b border-[#E0E3EB',
            { 'border-b-0': key === todoList.list.length - 1 },
          ]"
          v-for="(item, key) in todoList.list"
          :key="item.id"
        >
          <div class="flex items-start">
            <div class="basis-[55%]">
              <div class="font-semibold text-[10px] text-[#686D7B]">
                {{ item.text }}
              </div>
              <div class="flex items-center gap-x-2.5">
                <div class="w-2 h-2 rounded-full bg-[#FFC805]"></div>
                <div class="text-sm font-semibold">{{ item.text }}</div>
                <ChevronDown />
              </div>
              <div class="mt-1.5 text-sm text-[#686D7B]">Текст</div>
            </div>
            <div class="flex items-center gap-x-2 basis-[15%]">
              <Calendar />
              <div class="">
                <div class="font-semibold text-[10px] text-[#686D7B]">
                  {{ item.text }}
                </div>
                <div class="font-semibold text-sm">{{ item.difTime }}</div>
              </div>
            </div>
            <div class="basis-[12%]">
              <div class="font-semibold text-[10px] text-[#686D7B]">
                {{ item.text }}
              </div>
              <div class="font-semibold text-sm">{{ item.time }}</div>
            </div>
            <div class="basis-[8%]">
              <div class="font-semibold text-[10px] text-[#686D7B]">
                Итого, $
              </div>
              <div class="font-semibold text-sm">{{ item.price }}</div>
            </div>
            <div class="flex items-center gap-x-6 mt-1">
              <Calendar />
              <Calendar />
              <Calendar />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ChevronDown from "@/icons/ChevronDown.vue";
import Calendar from "@/icons/Calendar.vue";
import { useState } from "@/composables/state";
export default {
  name: "App-Todo",
  setup() {
    const [isOpen, setIsOpen] = useState(false);
    return {
      isOpen,
      setIsOpen,
    };
  },
  components: {
    ChevronDown,
    Calendar,
  },
  props: {
    todoList: {
      type: Object,
      default() {
        return {};
      },
    },
  },
};
</script>
