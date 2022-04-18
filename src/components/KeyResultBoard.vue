<script>
import "../assets/style/keyResult.scss"

export default {
    data () {
        return{
            progressMargin: 0,
            transition: 0.3,
        }
    },

    methods:{
        slideLeft(){
            this.progressMargin -= 20
        },
        slideRight(){
            this.progressMargin += 20
        },

    },

}
</script>
<template>
    <div class="keyResultBoard">
        <div class="keyResultBoard__topBar">
            <div class="keyResultBoard__topBar-leftContent">
                <div class="keyResultBoard__topBar-leftContent-tab">
                    <h1>Key Result Board</h1>
                    <img id="downIcons" src="../assets/icons/keyResultIcons/downIcon.svg" alt="">
                    <img id="newIcons" src="../assets/icons/keyResultIcons/New.svg" alt="">
                </div>
            </div>
            <div class="keyResultBoard__topBar-rightContent">
                <button>Add Widget</button>
            </div>
        </div>
        <div class="keyResultBoard__table">
            <div class="keyResultBoard__table-top">
                <div class="keyResultBoard__table-top-title">
                    <img src="../assets/icons/keyResultIcons/logo.png" alt="">
                    <h1>Key Result Board</h1>
                </div>
                <div class="keyResultBoard__table-top-filters">
                    <div class="keyResultBoard__table-top-filters-time">
                        <h1>Time</h1>
                        <h2>All Times</h2>
                    </div>
                    <div class="keyResultBoard__table-top-filters-completed">
                        <h1>Filter</h1>
                        <h2>Completed</h2>
                    </div>
                    <div class="keyResultBoard__table-top-filters-icon">
                        <img src="../assets/icons/keyResultIcons/settings.svg" alt="">
                    </div>
                </div>
            </div>
            <div class="keyResultBoard__table-content">
                <table class="table-auto  w-full">
                <thead>
                    <tr class="grayColor">
                    <th>Key Result</th>
                    <th>Start</th>
                    <th>Target</th>
                    <th>Current</th>
                    <th>Check in Progress</th>
                    <th>Owners</th>
                    <th>Last Check in</th>
                    </tr>
                </thead>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                <tbody class="text-center h-[50px]">
                    <tr>
                    <td class="w-[130px]">NPS</td>
                    <td>20</td>
                    <td>100</td>
                    <td class="current">
                        <img src="../assets/icons/keyResultIcons/current.svg" alt="">
                        100
                        </td>
                    <td>
                        <div class="keyResultBoard__table-content-parent">
                            <img src="../assets/icons/keyResultIcons/leftIcon.svg" @click="slideLeft" alt="">
                                <div class="keyResultBoard__table-content-parent-progress">
                                    <div class="keyResultBoard__table-content-parent-progress-info"
                                    v-bind:style="{ marginLeft: progressMargin + 'px', transition : transition + 's'}"
                                    >
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}" >0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FF8C8C'}">0</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFCA8C'}">60</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#FFFA8C'}">79</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                            <div class="info" :style="{backgroundColor: '#7FCB3D'}">100</div>
                                    </div>
                                </div>
                            <img src="../assets/icons/keyResultIcons/rightIcon.svg" @click="slideRight">
                        </div>
                    </td>
                    <td class="owners">
                        <img src="../assets/icons/keyResultIcons/owners.svg">
                    </td>
                    <td>10 -> 100</td>
                    </tr>
                </tbody>
                </table>
            </div>
        </div>
    </div>
</template>