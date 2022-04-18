<script>
import "../assets/style/menu.scss";
export default{
    data() {
        return {
        }
    }
}
</script>


<template>
    <div class="leftBar">
        <div class="leftBar__userInfo">
            <img src="../assets/images/owners.png" alt="">
            <h1>Ali Furkan</h1>
        </div>  
        <div class="leftBar__menu">
            <h4>Menu</h4>
            <ul>
                <li> <img src="../assets/icons/menuIcons/Tasks.svg"> <span>Tasks</span></li>
                <li> <img src="../assets/icons/menuIcons/Projects.svg"> <span>Projects</span></li>
                <li> <img src="../assets/icons/menuIcons/Meetings.svg"> <span>Meetings</span></li>
                <li  id="active"> <img src="../assets/icons/menuIcons/KeyResult.svg"> <span>Key Result Board</span></li>
                <li> <img src="../assets/icons/menuIcons/Settings.svg"> <span>Settings</span></li>
                <li> <img src="../assets/icons/menuIcons/Tasks.svg"> <span>Tasks</span></li>
                <li> <img src="../assets/icons/menuIcons/Projects.svg"> <span>Projects</span></li>
                <li> <img src="../assets/icons/menuIcons/Meetings.svg"> <span>Meetings</span></li>
                <li> <img src="../assets/icons/menuIcons/Settings.svg"> <span>Settings</span></li>
            </ul>
        </div>
    </div>
</template>
