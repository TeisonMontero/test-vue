<script>
import axios from 'axios'

const requestOptions = (config) => ({
    ...config,
    headers: {
        'Content-Type': 'application/json'
    },
})

const API = axios.create({
    baseURL: process.env.VUE_APP_API_URL
})

API.interceptors.request.use(requestOptions)

export default {
    name: 'API'
}
</script>
