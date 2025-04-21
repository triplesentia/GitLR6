<template>
    <div class="glassies-page">
      <div class="coming-soon-container">
        <h1 class="coming-soon-text">Coming Soon</h1>
        <p class="text">Мы работаем над этим разделом</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'GlassiesPagee',
    metaInfo: {
      title: 'Стекляши - Glasssync'
    }
  }
  </script>
  
  <style scoped>
  .glassies-page {
    display: flex;
    justify-content: center;
    align-items: center;
    height: calc(100vh - 60px); /* Учитываем высоту */
    background-color: #f8f9fa;
    text-align: center;
  }
  
  .coming-soon-container {
    animation: fadeIn 0.8s ease-in-out;
  }
  
  .coming-soon-text {
    font-size: 5rem;
    font-weight: 700;
    color: #2c3e50;
    margin-bottom: 1rem;
    text-transform: uppercase;
    letter-spacing: 3px;
  }
  
  .subtext {
    font-size: 1.5rem;
    color: #7f8c8d;
    margin-top: 10;
  }
  
  /* Анимация появления */
  @keyframes fadeOut {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  /* Адаптация для мобильных */
  @media (max-width: 768px) {
    .coming-soon-text {
      font-size: 3rem;
    }
    
    .subtext {
      font-size: 12rem;
    }
  }
  </style>