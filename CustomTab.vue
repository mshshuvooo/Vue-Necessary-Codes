<script setup>
import { ref } from "vue";
const openTab = ref(1);
const toggleTabs = (tabNumber) => {
    openTab.value = tabNumber
}
</script>

<template>
    <div class="flex flex-wrap">
        <div class="w-full">
            <ul class="flex mb-0 list-none flex-wrap pt-3 pb-4 flex-row">
                <li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
                <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal" :class="{'text-pink-600 bg-white': openTab !== 1, 'text-white bg-pink-600': openTab === 1}" @click="toggleTabs(1)">
                    Profile
                </a>
                </li>
                <li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
                <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal" :class="{'text-pink-600 bg-white': openTab !== 2, 'text-white bg-pink-600': openTab === 2}" @click="toggleTabs(2)">
                    Settings
                </a>
                </li>
                <li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
                <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal" :class="{'text-pink-600 bg-white': openTab !== 3, 'text-white bg-pink-600': openTab === 3}" @click="toggleTabs(3)">
                    Options
                </a>
                </li>
            </ul>
            <div class="relative flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded">
                <div class="px-4 py-5 flex-auto">
                    <div class="tab-content tab-space">
                        <div :class="{'hidden': openTab !== 1, 'block': openTab === 1}">
                        <p>
                            Collaboratively administrate empowered markets via
                            plug-and-play networks. Dynamically procrastinate B2C users
                            after installed base benefits.
                            <br />
                            <br />
                            Dramatically visualize customer directed convergence
                            without revolutionary ROI.
                        </p>
                        </div>
                        <div :class="{'hidden': openTab !== 2, 'block': openTab === 2}">
                        <p>
                            Completely synergize resource taxing relationships via
                            premier niche markets. Professionally cultivate one-to-one
                            customer service with robust ideas.
                            <br />
                            <br />
                            Dynamically innovate resource-leveling customer service for
                            state of the art customer service.
                        </p>
                        </div>
                        <div :class="{'hidden': openTab !== 3, 'block': openTab === 3}">
                        <p>
                            Efficiently unleash cross-media information without
                            cross-media value. Quickly maximize timely deliverables for
                            real-time schemas.
                            <br />
                            <br />
                            Dramatically maintain clicks-and-mortar solutions
                            without functional solutions.
                        </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

