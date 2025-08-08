<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Panel de Control - Rey del Brownie</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Inter from Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
    <!-- Chart.js for charts -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-gray-100">

    <div class="flex h-screen bg-gray-100">
        <!-- Sidebar -->
        <div class="hidden md:flex flex-col w-64 bg-stone-800 text-white shadow-xl">
            <!-- Sidebar Header -->
            <div class="flex items-center justify-center h-28 rounded-full bg-white w-28 mx-auto shadow-md">
                <img src="./logo.jpg" alt="Rey del Brownie Logo" class="h-24 rounded-full">
            </div>

            <!-- Sidebar Nav -->
            <nav class="flex-1 px-4 py-8 space-y-2">
                <a href="#" class="flex items-center px-4 py-3 rounded-lg hover:bg-stone-700 transition-colors duration-200">
                    <i class="fas fa-chart-line w-6 h-6 mr-3"></i>
                    <span>Dashboard</span>
                </a>
                <a href="#" class="flex items-center px-4 py-3 rounded-lg hover:bg-stone-700 transition-colors duration-200">
                    <i class="fas fa-users w-6 h-6 mr-3"></i>
                    <span>Clientes</span>
                </a>
                <a href="#" class="flex items-center px-4 py-3 rounded-lg hover:bg-stone-700 transition-colors duration-200">
                    <i class="fas fa-box-open w-6 h-6 mr-3"></i>
                    <span>Productos</span>
                </a>
                <a href="#" class="flex items-center px-4 py-3 rounded-lg hover:bg-stone-700 transition-colors duration-200">
                    <i class="fas fa-receipt w-6 h-6 mr-3"></i>
                    <span>Pedidos</span>
                </a>
                <a href="#" class="flex items-center px-4 py-3 rounded-lg hover:bg-stone-700 transition-colors duration-200">
                    <i class="fas fa-user-circle w-6 h-6 mr-3"></i>
                    <span>Usuarios</span>
                </a>
                <a href="#" class="flex items-center px-4 py-3 rounded-lg hover:bg-stone-700 transition-colors duration-200">
                    <i class="fas fa-cogs w-6 h-6 mr-3"></i>
                    <span>Ajustes</span>
                </a>
            </nav>
        </div>

        <!-- Main Content Area -->
        <div class="flex-1 flex flex-col overflow-hidden">
            <!-- Top Bar -->
            <header class="flex items-center justify-between px-6 py-4 bg-white shadow-md">
                <div class="text-2xl font-semibold text-gray-800">
                    Dashboard
                </div>
                <div class="flex items-center space-x-4">
                    <div class="relative">
                        <span class="absolute top-0 right-0 h-2 w-2 rounded-full bg-pink-500 ring-2 ring-white"></span>
                        <a href="#" class="text-gray-500 hover:text-stone-500">
                            <i class="fas fa-bell text-xl"></i>
                        </a>
                    </div>
                    <a href="#" class="flex items-center space-x-2 text-gray-500 hover:text-stone-500">
                        <i class="fas fa-user-circle text-xl"></i>
                        <span>Admin</span>
                    </a>
                </div>
            </header>

            <!-- Main Content -->
            <main class="flex-1 overflow-x-hidden overflow-y-auto bg-gray-100 p-6">
                <!-- Metrics Section -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
                    <!-- Metric Card 1 -->
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                        <div class="flex items-center justify-between">
                            <h4 class="text-lg font-semibold text-gray-500">Brownies Vendidos</h4>
                            <i class="fas fa-cookie-bite text-2xl text-stone-500"></i>
                        </div>
                        <p class="mt-2 text-3xl font-bold text-gray-900">12,543</p>
                        <p class="text-sm text-gray-500 mt-1">+12% vs. mes anterior</p>
                    </div>

                    <!-- Metric Card 2 -->
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                        <div class="flex items-center justify-between">
                            <h4 class="text-lg font-semibold text-gray-500">Ingresos</h4>
                            <i class="fas fa-dollar-sign text-2xl text-stone-500"></i>
                        </div>
                        <p class="mt-2 text-3xl font-bold text-gray-900">$15,200</p>
                        <p class="text-sm text-gray-500 mt-1">+8% vs. mes anterior</p>
                    </div>

                    <!-- Metric Card 3 -->
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                        <div class="flex items-center justify-between">
                            <h4 class="text-lg font-semibold text-gray-500">Nuevos Clientes</h4>
                            <i class="fas fa-user-plus text-2xl text-stone-500"></i>
                        </div>
                        <p class="mt-2 text-3xl font-bold text-gray-900">45</p>
                        <p class="text-sm text-gray-500 mt-1">Nuevos clientes este mes</p>
                    </div>

                    <!-- Metric Card 4 -->
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
                        <div class="flex items-center justify-between">
                            <h4 class="text-lg font-semibold text-gray-500">Satisfacción</h4>
                            <i class="fas fa-star text-2xl text-stone-500"></i>
                        </div>
                        <p class="mt-2 text-3xl font-bold text-gray-900">9.8 / 10</p>
                        <p class="text-sm text-gray-500 mt-1">Calificación promedio</p>
                    </div>
                </div>
                
                <!-- Sales Chart Section -->
                <div class="bg-white rounded-lg shadow-md p-6 mb-8">
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Ventas del Último Mes</h3>
                    <canvas id="salesChart"></canvas>
                </div>

                <!-- Orders and Notifications Section -->
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
                    <!-- Pending Orders Section -->
                    <div class="lg:col-span-2 bg-white rounded-lg shadow-md p-6">
                        <h3 class="text-2xl font-bold text-gray-800 mb-4">Pedidos Pendientes</h3>
                        <div class="overflow-x-auto">
                            <table class="min-w-full divide-y divide-gray-200">
                                <thead class="bg-gray-50">
                                    <tr>
                                        <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">ID de Pedido</th>
                                        <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Cliente</th>
                                        <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Fecha</th>
                                        <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Estado</th>
                                        <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Acciones</th>
                                    </tr>
                                </thead>
                                <tbody class="bg-white divide-y divide-gray-200">
                                    <tr>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900">#RDBC-001</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">Maria Lopez</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">2024-10-27</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm text-yellow-500 font-semibold">Pendiente</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-right text-sm font-medium">
                                            <a href="#" class="text-indigo-600 hover:text-indigo-900">Ver Detalles</a>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm font-medium text-gray-900">#RDBC-002</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">Juan Perez</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">2024-10-26</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-sm text-yellow-500 font-semibold">Pendiente</td>
                                        <td class="px-6 py-4 whitespace-nowrap text-right text-sm font-medium">
                                            <a href="#" class="text-indigo-600 hover:text-indigo-900">Ver Detalles</a>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>

                    <!-- Notifications Section -->
                    <div class="lg:col-span-1 bg-white rounded-lg shadow-md p-6">
                        <h3 class="text-2xl font-bold text-gray-800 mb-4">Notificaciones</h3>
                        <ul class="space-y-4">
                            <li class="p-4 bg-gray-50 rounded-lg flex items-start">
                                <div class="flex-shrink-0 mt-1">
                                    <i class="fas fa-exclamation-circle text-lg text-yellow-500"></i>
                                </div>
                                <div class="ml-3">
                                    <p class="font-semibold text-gray-900">Alerta: Bajo stock de nueces.</p>
                                    <p class="text-sm text-gray-500">El inventario de nueces ha caído por debajo del umbral de seguridad.</p>
                                </div>
                            </li>
                            <li class="p-4 bg-gray-50 rounded-lg flex items-start">
                                <div class="flex-shrink-0 mt-1">
                                    <i class="fas fa-check-circle text-lg text-green-500"></i>
                                </div>
                                <div class="ml-3">
                                    <p class="font-semibold text-gray-900">Nuevo cliente registrado.</p>
                                    <p class="text-sm text-gray-500">Se ha registrado un nuevo cliente en el sistema.</p>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </main>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Genera datos de ejemplo para el gráfico de ventas
            const labels = [];
            const data = [];
            for (let i = 29; i >= 0; i--) {
                const date = new Date();
                date.setDate(date.getDate() - i);
                labels.push(date.toLocaleDateString('es-ES', { day: 'numeric', month: 'short' }));
                data.push(Math.floor(Math.random() * 200) + 50); // Datos de ventas aleatorios
            }

            const ctx = document.getElementById('salesChart').getContext('2d');
            const salesChart = new Chart(ctx, {
                type: 'line',
                data: {
                    labels: labels,
                    datasets: [{
                        label: 'Ventas Diarias ($)',
                        data: data,
                        borderColor: '#A0522D', // Brown color
                        backgroundColor: 'rgba(160, 82, 45, 0.2)',
                        borderWidth: 2,
                        tension: 0.4,
                        fill: true
                    }]
                },
                options: {
                    responsive: true,
                    scales: {
                        x: {
                            display: true,
                            title: {
                                display: true,
                                text: 'Fecha'
                            }
                        },
                        y: {
                            display: true,
                            title: {
                                display: true,
                                text: 'Ventas ($)'
                            }
                        }
                    },
                    plugins: {
                        legend: {
                            display: false
                        }
                    }
                }
            });
        });
    </script>
</body>
</html>
