
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'line',
    data: {
        labels: ['231', '232', '233', '234'],
        datasets: [{
            label: 'عدد الطلاب',
            data: [3311, 3426, 2801, 2605], // قمت بوضع قيمة صفر للترم 234 حتى لا يتم رسمه في البيان
            borderColor: 'rgba(255, 99, 132, 1)',
            backgroundColor: 'rgba(255, 99, 132, 0.2)',
            borderWidth: 1
        },
        {
            label: 'الإيرادات',
            data: [7187910000, 7335065000, 6033663000, 6544394500], // قمت بوضع قيمة صفر للترم 234 حتى لا يتم رسمه في البيان
            borderColor: 'rgba(54, 162, 235, 1)',
            backgroundColor: 'rgba(54, 162, 235, 0.2)',
            borderWidth: 1
        },
        {
            label: 'النفقات',
            data: [6969540800, 6749239400, 5887325500, 5459557200], // قمت بوضع قيمة صفر للترم 234 حتى لا يتم رسمه في البيان
            borderColor: 'rgba(75, 192, 192, 1)',
            backgroundColor: 'rgba(75, 192, 192, 0.2)',
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
    }
});
