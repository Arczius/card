<span>{time}</span>


<script>
let time = getCurrentTime()
function getCurrentTime(){
    return new Date().toLocaleString('en-US', {timeZone: "Europe/Amsterdam", timeStyle: "medium"})
}
const timer = setInterval(() => {
    time = getCurrentTime()
}, 1000)
</script>