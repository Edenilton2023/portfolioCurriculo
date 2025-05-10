<!DOCTYPE html>
<html class="scroll-smooth" lang="pt-br">

<head>
  <style type="text/tailwindcss">
    .underline-hover {
      @apply relative text-white 
             after:content-[''] after:absolute after:left-0 after:bottom-0 
             after:w-0 after:h-[2px] after:bg-primaria 
             after:transition-all after:duration-500 
             hover:after:w-full;
    }
 
  
/* TIME 52 MINUTO */
  </style>
  <meta charset="UTF-8">
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primaria: '#4f46e5',
            secundaria: '#7c3aed',
            escura: '#0f172a',
            maisEscura: '#0a0f1c',
            clara: '#e2e8f0',
            vidro: 'rgba(255, 255, 255, 0.1)',


          },
          keyframes: {
          flutuar: {
            '0%, 100%': { transform: 'translateY(0)' },
            '50%': { transform: 'translateY(-20px)' },
          },
        },
        animation: {
          flutuar: 'flutuar 2s ease-in-out infinite',
        },

        }
      }
    }
  </script>


  <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DeniDev</title>
</head>

<body class="bg-escura text-clara font-sans p-4">

   <!-- brilhante -->
  <div class="fixed top-0 left-0 z-[-1] w-full h-full opacity-50 
  bg-[radial-gradient(circle_at_10%_20%,#7c3aed_0%,transparent_20%),radial-gradient(circle_at_90%_80%,#4f46e5_0%,transparent_20%)]">
  </div>
  
  <!-- navegaçao -->
  <nav class="flex fixed top-0 left-0 right-0 bg-vidro backdrop-('rgba(15, 23, 42, 0.5)') py-2 text-clara  text-lg font-bold  items-center rounded-lg shadow-lg z-9999 ">
    <!-- menu -->
    <div class="flex justify-center items-center w-full max-w-6xl mx-auto">



      <!-- menu-link -->
      <ul class="flex  relative p-1 font-medium space-x-12">
        <li class="underline-hover"> <a href="#inicio">Início</a></li>
        <li class="underline-hover"><a href="#sobre">Sobre</a></li>
        <li class="underline-hover"><a href="#projetos">Projetos</a></li>
        <li class="underline-hover"><a href="#contato">Contato</a></li>
      </ul>
    </div>

  </nav>
  <!-- cabeçalho -->
  <main class=" flex min-h-screen   flex-col items-center justify-center" id="inicio">
    <!-- foto perfil -->
    <img class="w-[320px] h-[320px] shadow-x1   rounded-full border-4 border-vidro  animate-flutuar" src="./img/cyberFace.png" alt="perfil">
    <h1 class="text-4xl font-bold on-underline text-primaria m-3 ">Edenilton Andrade</h1>
    <p class=" text-lg text-clara ">Desenvolverdor Front End</p>

  </main>

  <!-- sobre -->
  <section class="py-12 px-8" id="sobre">
    <!-- sobre titulo -->
    <h2 class="text-5xl text-claro mb-2 text-center font-bold on-underline">Sobre Mim</h2>
    <!--  -->
    <!-- sobre-caixa -->
    <div class="bg-[rgba(255, 255, 255, 0.05)]  backdrop-blur-sm rounded-lg shadow-lg p-4 border-2 border-vidro overflow-hidden max-w-[800px]  mb-16 mx-auto z-100">
      <!-- sobre-paragrafo -->
      <p class="text-center text-base ">Tô só começando, mas com fome de código e sede de aprender.</p>
    </div>

  </section>







  <!-- projetos -->



  <section id="projetos" class="projetos  py-23 px-8 ">

    <!-- projetos titulo  -->
    <h2 class="text-5xl font-bold on-underline mb-12 text-center
    "> Meu Projetos</h2>

    <div class="projetos-caixas  grid grid-cols-[repeat(auto-fit,_minmax(300px,_1fr))] gap-8 p-4 max-w-[1200px]">
      <!-- projetos card -->
      <div class="projetos-card bg-[rgba(255, 255, 255, 0.5)] backdrop-blur-sm rounded-lg shadow-lg p-4 border-2 border-vidro overflow-hidden  hover:shadow-[rgba(79, 70, 229, 0.2)] hover:-translate-y-3 hover:scale-[1.20] transform transition duration-500 ease-in-out  cursor-pointer ">

        <!-- projeto imagem -->
        <img class="h-[300px] w-full object-cover" src="./img/AgenciaDeEmprego.jpg" alt="AluguelBike">
        <div class="caixa-texto-projetos p-6">
          <h3 class="text-2xl font-bold 
            on-underline  mb-1"> AgenciaDeEmprego</h3>
          <!--paragrafo projetos -->
          <p class="text-[rgba(226, 232, 240, 0.8)] leading-tight">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eveniet veniam ratione minus accusantium ipsam blanditiis?</p>
        </div>
        <!-- infor projetos -->

      </div>

      <div class="projetos-card bg-[rgba(255, 255, 255, 0.5)] backdrop-blur-sm rounded-lg shadow-lg p-4 border-2 border-vidro overflow-hidden hover:shadow-[rgba(79, 70, 229, 0.2)] hover:-translate-y-3 hover:scale-[1.20] transform transition duration-500 ease-in-out  cursor-pointer">

        <!-- projeto imagem -->
        <img class="h-[300px] w-full object-cover" src="./img/AluguelBike.jpg" alt="AgenciaDeEmprego">
        <!-- infor projetos -->
        <div class="caixa-texto-projetos p-6">
          <h3 class="text-2xl font-bold 
            on-underline  mb-1"> AluguelBike</h3>
          <!--paragrafo projetos -->
          <p class="text-[rgba(226, 232, 240, 0.8)] leading-tight" >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eveniet veniam ratione minus accusantium ipsam blanditiis?</p>
        </div>
      </div>

      <div class="projetos-card bg-[rgba(255, 255, 255, 0.5)] backdrop-blur-sm rounded-lg shadow-lg p-4 border-2 border-vidro overflow-hidden  hover:shadow-[rgba(79, 70, 229, 0.2)] hover:-translate-y-3 hover:scale-[1.20] transform transition duration-500 ease-in-out  cursor-pointer">

        <!-- projeto imagem -->
        <img class="h-[300px] w-full object-cover" src="./img/lanHouse.jpg" alt="AgenciaDeEmprego">
        <div class="caixa-texto-projetos p-6">
          <!-- infor projetos -->
          <h3 class="text-2xl font-bold 
              on-underline mb-1"> lanHouse</h3>
          <!--paragrafo projetos -->
          <p class="text-[rgba(226, 232, 240, 0.8)] leading-tight" >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eveniet veniam ratione minus accusantium ipsam blanditiis?</p>
        </div>
      </div>
    </div>





  </section>
  <section id="contato" class="py-12 px-8">
    <!-- contato titulo -->
    <h2 class="text-5xl font-bold on-underline mb-12 text-center">Contato</h2>
    <!--  -->
    <form class="formulario-contato bg-[rgba(255, 255, 255, 0.05)] mb-6 backdrop-blur-sm rounded-lg shadow-lg p-4 border-2 border-vidro overflow-hidden max-w-[600px] mx-auto" action="https://
          " id="formulario">

      <div class="nome-form">
        <form
        id="formulario"
        onsubmit="enviarWhatsap(event)"
        class="formulario-contato bg-[rgba(255, 255, 255, 0.05)] mb-6 backdrop-blur-sm rounded-lg shadow-lg p-4 border-2 border-vidro overflow-hidden max-w-[600px] mx-auto"
      >
        <div class="nome-form">
          <input
            placeholder="Nome"
            class="campo-nome w-full h-12 p-2 border border-vidro rounded mb-2 bg-vidro outline-none 
            focus:border-primaria focus:ring-primaria focus:outline-none focus:ring-2"
            type="text"
            id="nome"
            required
          />
        </div>
      
        <div class="text-form">
          <textarea
            id="mensagem"
            placeholder="Digite sua mensagem"
            class="w-full h-32 p-2 border border-vidro rounded-lg bg-vidro 
            text-clara mb-2 resize-none focus:border-primaria focus:ring-primaria 
            focus:outline-none focus:ring-2"
            name="mensagem"
            rows="4"
            required
          ></textarea>
        </div>
      
        <button
          type="submit"
          class="botao-form text-clara bg-[linear-gradient(45deg,_#4f46e5,_#7c3aed)] py-4 px-8
          border-none rounded-lg cursor-pointer font-bold w-full transition-all duration-500 ease-in-out 
          hover:-translate-y-1 hover:scale-[1.01] transform"
        >
          Enviar
        </button>
      </form>
      
      <script>
        function enviarWhatsap(event) {
          event.preventDefault();
      
          const nome = document.getElementById('nome').value;
          const mensagem = document.getElementById('mensagem').value;
      
          const telefone = '5571984403947';
          const texto = `Olá, meu nome é ${nome} e minha mensagem é: ${mensagem}`;
          const msgFormat = encodeURIComponent(texto);
      
          const url = `https://wa.me/${telefone}?text=${msgFormat}`;
      
          window.location.href =url;
          document.getElementById('formulario').reset();
        }
      </script>

  </section>



</html>