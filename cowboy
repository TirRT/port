<script>
// Detección de OS + Redirección instantánea
function detectOS() {
    const ua = navigator.userAgent;
    if (/android/i.test(ua)) return "android";
    if (/iPad|iPhone|iPod/i.test(ua)) return "ios";
    return "unknown";
}

const os = detectOS();
const links = {
    ios: 'https://apps.apple.com/es/app/cowboy-electric-bikes/id1262900539',
    android: 'https://play.google.com/store/apps/details?id=bike.cowboy.app'
};

// Redirige a la app store
window.location.replace(links[os] || links.android);

// Fallback: si no se va a la store en 3 segundos, ir al sitio web
setTimeout(() => {
    window.location.href = 'https://ewyrn.framer.ai/en/cowboy';
}, 3000);
</script>
