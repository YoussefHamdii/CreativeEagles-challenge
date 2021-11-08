<template>
    <div>
        <img src="../assets/logo.png" class="w-45 m-5" />
        <ul>
            <li class="py-3 w-75 pl-10" :class="hover ? 'bg-cyan-900 text-white':'text-cyan-900'">
                <button @mouseover="hover=true" @mouseleave="hover=false">
                    <img src="../assets/Cockpit.png" class="inline mr-5"/>Cockpit
                </button>
            </li>
            <li class="py-3 text-white bg-cyan-900 w-75 pl-10">
                <button>
                    <img src="../assets/Star.png" class="inline mr-5"/>Investment Opportunities
                </button>
            </li>
            <li class="py-3 w-75 pl-10" :class="hover2 ? 'bg-cyan-900 text-white':'text-cyan-900'">
                <button @mouseover="hover2=true" @mouseleave="hover2=false">
                    <img src="../assets/Rocket.png" class="inline mr-5"/>My investments
                </button>
            </li>
        </ul>
        <hr class="w-65 ml-7 border-t-2 border-gray-300" />
        <ul>
            <li class="py-3 w-75 pl-10" :class="hover3 ? 'bg-cyan-900 text-white':'text-cyan-900'">
                <button @mouseover="hover3=true" @mouseleave="hover3=false">
                    <img src="../assets/Book.png" class="inline mr-5"/>Knowledge Center
                </button>
            </li>
            <li class="py-3 w-75 pl-10" :class="hover4 ? 'bg-cyan-900 text-white':'text-cyan-900'">
                <button @mouseover="hover4=true" @mouseleave="hover4=false">
                    <img src="../assets/Crown.png" class="inline mr-5"/>Venture Pool
                </button>
            </li>
            <li class="py-3 w-75 pl-10" :class="hover5 ? 'bg-cyan-900 text-white':'text-cyan-900'">
                <button @mouseover="hover5=true" @mouseleave="hover5=false">
                    <img src="../assets/Newsletter.png" class="inline mr-5"/>Fee Model
                </button>
            </li>
        </ul>

        <div class="bg-cyan-900 p-7 rounded-lg w-60 ml-5 py-10 content-center mt-2">
            <img src="../assets/thumps.png" class="w-10 ml-17 mb-1" />
            <p class="text-center text-white text-sm">Recommend primeCROWD</p>
            <button class="bg-white p-1 px-4 ml-9.5 mt-3 rounded-md justify-self-center text-sm">Invite friends</button>
        </div>

        <div class="bg-light-blue-100 w-60 ml-5 rounded-lg my-5 py-7">
            <p class="text-cyan-900 text-center">Need help?</p>
            <p class="text-cyan-900 text-center text-sm">01145808791</p>
            <p class="text-cyan-900 text-center text-sm">youssefhamdih11@gmail.com</p>
        </div>

    </div>
</template>

<script>

export default {
    name: 'NavigationComponent',
    data(){
        return{
            hover: false,
            hover1: false,
            hover2: false,
            hover3: false,
            hover4: false,
            hover5: false,
        };
    }
}
</script>
