<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Estudios IA Camoens: educación, creatividad e innovación.">
  <title>ESTUDIOS IA CAMOENS · Aula virtual</title>
  <link rel="icon" href="data:,">
  <style>
    :root{color-scheme:dark;--fondo:#08111f;--panel:#111e32;--texto:#f5f7ff;--secundario:#c3cee1;--azul:#75a7ff;--verde:#83f0d0;--borde:#304563}
    *{box-sizing:border-box}
    [hidden]{display:none!important}
    body{margin:0;background:var(--fondo);color:var(--texto);font-family:Arial,sans-serif;line-height:1.6}
    a{color:var(--azul)}
    button,input{font:inherit}
    button,a,input,summary{-webkit-tap-highlight-color:transparent}
    :focus-visible{outline:3px solid var(--verde);outline-offset:4px}
    .saltar{position:absolute;left:16px;top:-100px;z-index:10;background:var(--texto);color:var(--fondo);padding:12px}
    .saltar:focus{top:12px}
    header{padding:24px 8%;background:#101d32;border-bottom:1px solid var(--borde);display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:20px}
    .logo{font-weight:900;font-size:21px;color:var(--azul);text-decoration:none;overflow-wrap:anywhere}
    nav{display:flex;flex-wrap:wrap;gap:8px 22px}
    nav a{color:#dbe5ff;text-decoration:none;padding:8px 0}
    nav a:hover{text-decoration:underline}
    section{padding:55px 8%;scroll-margin-top:20px}
    .hero{padding:85px 8%;background:radial-gradient(ellipse at top right,#244b85,var(--fondo) 65%)}
    .tag{color:var(--verde);font-weight:bold;letter-spacing:.08em;font-size:14px}
    h1{font-size:clamp(36px,7vw,70px);line-height:1.08;margin:20px 0}
    h2{font-size:clamp(25px,4vw,30px);line-height:1.25;margin:0 0 16px}
    h3{line-height:1.35}
    .hero p{font-size:19px;color:var(--secundario);max-width:650px;line-height:1.7}
    .btn,button{display:inline-block;padding:13px 20px;border-radius:10px;border:1px solid transparent;background:var(--azul);color:var(--fondo);font-weight:bold;text-decoration:none;cursor:pointer}
    .btn{margin-top:14px}
    button:hover:not(:disabled),.btn:hover{filter:brightness(1.08)}
    button:disabled{opacity:.6;cursor:wait}
    .secundario{background:transparent;color:var(--texto);border-color:var(--borde)}
    .cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(220px,100%),1fr));gap:20px}
    .card{background:var(--panel);border:1px solid var(--borde);border-radius:16px;padding:24px;min-width:0}
    .card p,.muted{color:var(--secundario)}
    .icon{color:var(--azul);line-height:1}.icon svg{width:34px;height:34px}.icono-titulo{width:30px;height:30px;vertical-align:-4px;color:var(--azul)}
    details{border-top:1px solid var(--borde);padding-top:12px}
    summary{cursor:pointer;color:var(--azul);font-weight:bold}
    .acceso-contenedor{max-width:540px;margin:0 auto;background:#17243b;padding:clamp(20px,5vw,32px);border:1px solid var(--borde);border-radius:18px}
    .centrado{text-align:center}
    .modos{display:flex;flex-wrap:wrap;gap:10px;margin:24px 0}
    .modos button{flex:1;min-width:130px}
    .modos button[aria-pressed="false"]{background:transparent;color:var(--secundario);border-color:var(--borde)}
    label{display:block;font-weight:bold;margin-top:16px}
    input{display:block;width:100%;min-width:0;padding:12px;margin:8px 0;border:1px solid #7e91ae;border-radius:8px;background:#0c1729;color:var(--texto)}
    input::placeholder{color:#aebbd0}
    .ayuda{font-size:14px;color:var(--secundario);margin:6px 0 18px}
    .ancho{width:100%;margin-top:12px}
    .mensaje{margin:20px 0 0;overflow-wrap:anywhere}
    .mensaje:empty{display:none}
    .mensaje[data-tipo="error"]{color:#ffb7b7}
    .mensaje[data-tipo="exito"]{color:var(--verde)}
    #correo-sesion{overflow-wrap:anywhere;font-weight:bold;color:var(--verde)}
    .nota{background:#13233a;border-left:3px solid var(--azul);padding:14px 18px;color:var(--secundario)}
    footer{text-align:center;padding:30px 8%;color:#aebbd0;border-top:1px solid var(--borde)}
    @media(max-width:480px){header,section{padding-left:6%;padding-right:6%}.hero{padding:60px 6%}nav{gap:16px}.card{padding:20px}}
  </style>
</head>
<body>
  <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" width="0" height="0" style="position:absolute;overflow:hidden">
    <defs>
      <symbol id="icono-libro" viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M12 5v15M3 4c4-1 6 0 9 2 3-2 5-3 9-2v15c-4-1-6 0-9 2-3-2-5-3-9-2Z"/></g></symbol>
      <symbol id="icono-cohete" viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M8 15c2-7 7-12 13-12 0 6-5 11-12 13ZM8 15l-4-1 3-5h4M9 16l1 4 5-3v-4M6 17l-3 4 4-2"/><circle cx="16" cy="8" r="2"/></g></symbol>
      <symbol id="icono-pizarra" viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3h18v13H3ZM12 16v5M8 21l4-3 4 3M7 7h10M7 11h6"/></g></symbol>
      <symbol id="icono-grado" viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="m2 8 10-5 10 5-10 5ZM6 10v7c4 3 8 3 12 0v-7M22 8v8"/></g></symbol>
    </defs>
  </svg>

  <a class="saltar" href="#contenido">Saltar al contenido</a>
  <header>
    <a class="logo" href="#inicio">✦ ESTUDIOS IA CAMOENS</a>
    <nav aria-label="Navegación principal">
      <a href="#inicio">Inicio</a><a href="#acceso">Aula virtual</a><a href="#contacto">Contacto</a>
    </nav>
  </header>
  <main id="contenido">
    <section class="hero" id="inicio" aria-labelledby="titulo">
      <div class="tag">APRENDE · CREA · DESCUBRE</div>
      <h1 id="titulo">Tu futuro<br>empieza aquí.</h1>
      <p>Bienvenido a ESTUDIOS IA CAMOENS, un espacio educativo para aprender, desarrollar proyectos y compartir ideas. ¡El próximo gran proyecto puede ser el tuyo!</p>
      <a class="btn" href="#acceso">Entrar al aula →</a>
    </section>
    <section id="servicios" aria-labelledby="titulo-servicios">
      <h2 id="titulo-servicios">Tu espacio de aprendizaje</h2>
      <p class="muted">Conoce las áreas del aula y lo que podrás encontrar en ellas.</p>
      <div class="cards">
        <article class="card"><div class="icon" aria-hidden="true"><svg><use href="#icono-libro"></use></svg></div><h3>Ejercicios y tareas</h3><p>Actividades para practicar y organizar tu trabajo académico.</p><details><summary>Ver información</summary><p>Las actividades y las entregas estarán disponibles cuando el centro publique sus contenidos. Todavía no hay tareas conectadas a esta página.</p></details></article>
        <article class="card"><div class="icon" aria-hidden="true"><svg><use href="#icono-cohete"></use></svg></div><h3>Proyectos</h3><p>Ideas, experiencias y retos para aprender creando.</p><details><summary>Ver información</summary><p>Este espacio está preparado para presentar proyectos educativos. El centro todavía no ha añadido un catálogo de proyectos.</p></details></article>
        <article class="card"><div class="icon" aria-hidden="true"><svg><use href="#icono-pizarra"></use></svg></div><h3>Zona docente</h3><p>Recursos y actividades para acompañar el aprendizaje.</p><details><summary>Ver información</summary><p>Los permisos docentes deben ser asignados por el centro. Crear una cuenta no concede permisos para administrar contenidos.</p></details></article>
        <article class="card"><div class="icon" aria-hidden="true"><svg><use href="#icono-grado"></use></svg></div><h3>Zona de estudiantes</h3><p>Tu primer paso para participar en el aula virtual.</p><a href="#acceso">Acceder a mi cuenta →</a></article>
      </div>
    </section>
    <section id="acceso" aria-labelledby="titulo-acceso">
      <div class="acceso-contenedor">
        <h2 id="titulo-acceso" class="centrado"><svg class="icono-titulo" aria-hidden="true"><use href="#icono-grado"></use></svg> Aula virtual</h2>
        <p id="descripcion-acceso" class="centrado muted">Inicia sesión o crea tu cuenta.</p>
        <noscript><p class="nota">Activa JavaScript en tu navegador para registrarte o iniciar sesión.</p></noscript>
        <div id="zona-formulario">
          <div class="modos" role="group" aria-label="Tipo de acceso">
            <button id="modo-login" type="button" aria-pressed="true" disabled>Iniciar sesión</button>
            <button id="modo-registro" type="button" aria-pressed="false" disabled>Crear cuenta</button>
          </div>
          <form id="formulario-acceso" novalidate>
            <label for="email">Correo electrónico</label>
            <input id="email" name="email" type="email" autocomplete="username" inputmode="email" autocapitalize="none" spellcheck="false" required placeholder="tu@correo.com" disabled>
            <label for="password">Contraseña</label>
            <input id="password" name="password" type="password" autocomplete="current-password" required aria-describedby="ayuda-password" disabled>
            <p class="ayuda" id="ayuda-password">Introduce la contraseña de tu cuenta.</p>
            <div id="confirmacion-contenedor" hidden>
              <label for="confirmacion">Repite la contraseña</label>
              <input id="confirmacion" name="confirmacion" type="password" autocomplete="new-password" disabled>
            </div>
            <button id="enviar" type="submit" class="ancho" disabled>Iniciar sesión</button>
          </form>
        </div>
        <div id="panel-sesion" hidden>
          <p>Has accedido con:</p>
          <p id="correo-sesion"></p>
          <p class="nota">Tu sesión está activa. Las tareas, proyectos y permisos del centro todavía no están conectados a esta versión del aula.</p>
          <a class="btn" href="#servicios">Consultar las áreas del aula</a>
          <button id="cerrar-sesion" class="ancho secundario" type="button" disabled>Cerrar sesión en este navegador</button>
        </div>
        <p id="mensaje-acceso" class="mensaje" role="status" aria-live="polite" aria-atomic="true">Preparando el acceso…</p>
        <button id="reintentar" type="button" class="ancho secundario" hidden>Volver a cargar</button>
      </div>
    </section>
    <section id="contacto" aria-labelledby="titulo-contacto">
      <h2 id="titulo-contacto">Construimos el futuro juntos</h2>
      <p>ESTUDIOS IA CAMOENS · Educación, creatividad e innovación.</p>
      <p class="muted">Para dudas sobre tu matrícula o acceso, consulta al profesorado del centro. Los datos de contacto oficiales aún no se han publicado en esta página.</p>
    </section>
  </main>
  <footer>© 2026 ESTUDIOS IA CAMOENS · Aprender para avanzar.</footer>

  <!--
  CONFIGURACIÓN Y PUESTA EN MARCHA
  1. Guarda este archivo como index.html en tu alojamiento web.
     Para una prueba local: python3 -m http.server 8000
     y abre http://localhost:8000/Estudios_IA_Camoens.html (o /index.html si lo renombraste).
  2. En Supabase > Authentication > URL Configuration establece tu Site URL
     y añade la dirección exacta de esta página a Redirect URLs.
  3. Habilita el proveedor Email y decide si los registros necesitan confirmación.
     Configura el correo saliente del proyecto para entregar las confirmaciones.
  4. La clave publishable siguiente es pública por diseño. No uses una secret o service_role.
  5. Este archivo implementa autenticación y una portada; no inventa tablas ni roles.
     Antes de añadir datos privados, crea las políticas RLS y los permisos en el servidor.
     Ocultar un panel en HTML no es un control de autorización.
  6. Necesita Internet. Incluye manejo de fallos de carga y conexión.
  -->
  <script>
  (() => {
    'use strict';
    const SUPABASE_URL = 'https://yzebqbuyliqczeswshqk.supabase.co';
    const SUPABASE_PUBLISHABLE_KEY = 'sb_publishable_Zjlfd1g9TErkZxMBlzNvlA_7N15XUgV';
    const SDK_URL = 'https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2.118.0/dist/umd/supabase.js';
    const $ = (id) => document.getElementById(id);
    const formulario = $('formulario-acceso');
    const email = $('email');
    const password = $('password');
    const confirmacion = $('confirmacion');
    const mensaje = $('mensaje-acceso');
    const enviar = $('enviar');
    const modoLogin = $('modo-login');
    const modoRegistro = $('modo-registro');
    const cerrar = $('cerrar-sesion');
    let cliente = null;
    let listo = false;
    let ocupado = false;
    let modo = 'login';
    let sesion = null;
    let revisionSesion = 0;
    // Capturar antes de que el SDK procese y limpie un enlace de autenticación.
    const fragmentoInicial = new URLSearchParams(window.location.hash.slice(1));
    const consultaInicial = new URLSearchParams(window.location.search);
    const errorEnRetorno = [fragmentoInicial, consultaInicial].some(
      (parametros) => parametros.has('error') || parametros.has('error_code')
    );

    function avisar(texto, tipo = 'info') {
      mensaje.textContent = texto;
      mensaje.dataset.tipo = tipo;
    }

    function actualizarControles() {
      const bloqueado = !listo || ocupado;
      for (const control of [modoLogin, modoRegistro, email, password, enviar]) {
        control.disabled = bloqueado || Boolean(sesion);
      }
      confirmacion.disabled = bloqueado || modo !== 'registro' || Boolean(sesion);
      cerrar.disabled = bloqueado || !sesion;
      formulario.setAttribute('aria-busy', String(ocupado));
      enviar.textContent = ocupado ? 'Procesando…' : modo === 'registro' ? 'Crear cuenta' : 'Iniciar sesión';
    }

    function mostrarSesion(nuevaSesion) {
      const anterior = sesion?.user?.id;
      sesion = nuevaSesion?.user ? nuevaSesion : null;
      $('zona-formulario').hidden = Boolean(sesion);
      $('panel-sesion').hidden = !sesion;
      $('descripcion-acceso').textContent = sesion ? 'Bienvenido a tu cuenta.' : 'Inicia sesión o crea tu cuenta.';
      $('correo-sesion').textContent = sesion?.user?.email || '';
      if (sesion || anterior) {
        password.value = '';
        confirmacion.value = '';
        confirmacion.setCustomValidity('');
      }
      actualizarControles();
    }

    function cambiarModo(nuevoModo) {
      if (ocupado || !listo || sesion) return;
      modo = nuevoModo;
      const registro = modo === 'registro';
      modoLogin.setAttribute('aria-pressed', String(!registro));
      modoRegistro.setAttribute('aria-pressed', String(registro));
      $('confirmacion-contenedor').hidden = !registro;
      confirmacion.required = registro;
      confirmacion.setCustomValidity('');
      password.value = '';
      confirmacion.value = '';
      password.autocomplete = registro ? 'new-password' : 'current-password';
      if (registro) password.minLength = 8;
      else password.removeAttribute('minlength');
      $('ayuda-password').textContent = registro
        ? 'Usa al menos 8 caracteres. El centro puede exigir una contraseña más segura.'
        : 'Introduce la contraseña de tu cuenta.';
      avisar('');
      actualizarControles();
    }

    function explicarError(error) {
      const mensajes = {
        invalid_credentials: 'El correo o la contraseña no son correctos.',
        email_not_confirmed: 'Confirma tu correo antes de iniciar sesión. Revisa también la carpeta de spam.',
        signup_disabled: 'El centro ha desactivado temporalmente la creación de cuentas.',
        user_already_exists: 'No se pudo crear la cuenta. Si ya la tienes, inicia sesión.',
        email_exists: 'No se pudo crear la cuenta. Si ya la tienes, inicia sesión.',
        email_address_invalid: 'Introduce un correo electrónico válido.',
        email_address_not_authorized: 'El servicio de correo del centro aún no permite enviar a esta dirección. Contacta con el centro.',
        weak_password: 'La contraseña no cumple la política de seguridad. Elige una más larga y difícil de adivinar.',
        over_email_send_rate_limit: 'Se han solicitado demasiados correos. Espera unos minutos antes de volver a intentarlo.',
        over_request_rate_limit: 'Hay demasiados intentos. Espera unos minutos y vuelve a probar.'
      };
      if (mensajes[error?.code]) return mensajes[error.code];
      if (error?.status === 429) return mensajes.over_request_rate_limit;
      if (!navigator.onLine || error?.name === 'AbortError' || error?.name === 'AuthRetryableFetchError' || error instanceof TypeError) {
        return 'No se pudo conectar con el servicio. Revisa tu conexión e inténtalo de nuevo.';
      }
      return 'No se pudo completar la operación. Inténtalo de nuevo; si continúa, consulta al centro.';
    }

    // El callback de onAuthStateChange solo actualiza la interfaz: no espera otras llamadas de Auth.
    function alCambiarSesion(evento, nuevaSesion) {
      revisionSesion += 1;
      mostrarSesion(nuevaSesion);
      if (ocupado) return;
      if (evento === 'SIGNED_OUT') avisar('La sesión se ha cerrado.');
      else if (evento === 'SIGNED_IN') avisar('Sesión iniciada correctamente.', 'exito');
    }

    async function enviarFormulario(evento) {
      evento.preventDefault();
      if (!listo || ocupado || sesion) return;
      email.value = email.value.trim();
      confirmacion.setCustomValidity('');
      if (modo === 'registro' && password.value.length < 8) {
        avisar('La contraseña debe tener al menos 8 caracteres.', 'error');
        password.focus();
        return;
      }
      if (modo === 'registro' && password.value !== confirmacion.value) {
        confirmacion.setCustomValidity('Las contraseñas no coinciden.');
      }
      if (!formulario.reportValidity()) return;
      if (!navigator.onLine) {
        avisar('No tienes conexión. Conéctate a Internet antes de continuar.', 'error');
        return;
      }
      const registro = modo === 'registro';
      const credenciales = { email: email.value, password: password.value };
      ocupado = true;
      actualizarControles();
      avisar(registro ? 'Creando tu cuenta…' : 'Comprobando tus datos…');
      try {
        const retorno = new URL(window.location.href);
        retorno.search = '';
        retorno.hash = '';
        const { data, error } = registro
          ? await cliente.auth.signUp({ ...credenciales, options: { emailRedirectTo: retorno.href } })
          : await cliente.auth.signInWithPassword(credenciales);
        if (error) throw error;
        password.value = '';
        confirmacion.value = '';
        if (data?.session) {
          mostrarSesion(data.session);
          avisar(registro ? 'Cuenta creada y sesión iniciada.' : '¡Has iniciado sesión correctamente!', 'exito');
          cerrar.focus();
        } else if (registro) {
          avisar('Solicitud de registro recibida. Si el registro procede, recibirás un correo de confirmación. Revisa también spam. Si ya tienes cuenta, inicia sesión.', 'exito');
        } else {
          avisar('No se recibió una sesión válida. Intenta iniciar sesión de nuevo.', 'error');
        }
      } catch (error) {
        avisar(explicarError(error), 'error');
      } finally {
        ocupado = false;
        actualizarControles();
        if (sesion) cerrar.focus();
      }
    }

    async function cerrarSesion() {
      if (!listo || ocupado || !sesion) return;
      ocupado = true;
      actualizarControles();
      avisar('Cerrando sesión…');
      try {
        const { error } = await cliente.auth.signOut({ scope: 'local' });
        if (error) throw error;
        mostrarSesion(null);
        formulario.reset();
        avisar('Has cerrado sesión en este navegador.', 'exito');
      } catch (error) {
        // Algunas versiones del SDK borran la sesión local aunque falle la revocación remota.
        // El evento SIGNED_OUT ya habrá actualizado la interfaz en ese caso.
        avisar(sesion
          ? 'No se pudo cerrar la sesión. ' + explicarError(error)
          : 'La sesión local se ha cerrado, pero no se pudo confirmar el cierre en el servidor. ' + explicarError(error), 'error');
      } finally {
        ocupado = false;
        actualizarControles();
        if (!sesion) email.focus();
      }
    }

    function cargarSDK() {
      if (window.supabase?.createClient) return Promise.resolve();
      return new Promise((resolve, reject) => {
        const script = document.createElement('script');
        const temporizador = setTimeout(() => terminar(new Error('sdk_timeout')), 15000);
        function terminar(error) {
          clearTimeout(temporizador);
          script.onload = null;
          script.onerror = null;
          if (error) { script.remove(); reject(error); }
          else resolve();
        }
        script.src = SDK_URL;
        script.async = true;
        script.onload = () => terminar(window.supabase?.createClient ? null : new Error('sdk_invalid'));
        script.onerror = () => terminar(new Error('sdk_unavailable'));
        document.head.appendChild(script);
      });
    }

    async function fetchConLimite(input, opciones = {}) {
      const controller = new AbortController();
      const senal = opciones.signal;
      const cancelar = () => controller.abort();
      if (senal?.aborted) cancelar();
      else senal?.addEventListener('abort', cancelar, { once: true });
      const temporizador = setTimeout(cancelar, 15000);
      try {
        return await fetch(input, { ...opciones, signal: controller.signal });
      } finally {
        clearTimeout(temporizador);
        senal?.removeEventListener('abort', cancelar);
      }
    }

    async function iniciar() {
      try {
        if (!['https:', 'http:'].includes(window.location.protocol)) {
          avisar('Para usar el acceso, abre esta página desde un alojamiento web o un servidor local; no directamente como archivo.', 'error');
          return;
        }
        const url = new URL(SUPABASE_URL);
        if (url.protocol !== 'https:' || !SUPABASE_PUBLISHABLE_KEY.startsWith('sb_publishable_')) {
          throw new Error('config_invalid');
        }
        try {
          await cargarSDK();
        } catch {
          avisar('No se pudo cargar el servicio de acceso. Revisa tu conexión y vuelve a cargar la página.', 'error');
          $('reintentar').hidden = false;
          return;
        }
        cliente = window.supabase.createClient(SUPABASE_URL, SUPABASE_PUBLISHABLE_KEY, {
          auth: { persistSession: true, autoRefreshToken: true, detectSessionInUrl: true },
          global: { fetch: fetchConLimite }
        });
        cliente.auth.onAuthStateChange(alCambiarSesion);
        const revisionInicial = revisionSesion;
        const { data, error } = await cliente.auth.getSession();
        if (error) throw error;
        if (revisionInicial === revisionSesion) mostrarSesion(data?.session || null);
        listo = true;
        actualizarControles();
        // Los enlaces de confirmación fallidos pueden devolver un error en la URL.
        if (errorEnRetorno) {
          avisar('El enlace de confirmación no es válido o ha caducado. Solicita ayuda al centro o utiliza un enlace de confirmación vigente.', 'error');
        } else {
          avisar(sesion ? 'Ya tienes una sesión iniciada.' : '', sesion ? 'exito' : 'info');
        }
      } catch {
        listo = false;
        actualizarControles();
        avisar('No se pudo preparar el acceso. Comprueba la conexión y la configuración del proyecto; después vuelve a cargar.', 'error');
        $('reintentar').hidden = false;
      }
    }

    modoLogin.addEventListener('click', () => cambiarModo('login'));
    modoRegistro.addEventListener('click', () => cambiarModo('registro'));
    formulario.addEventListener('submit', enviarFormulario);
    cerrar.addEventListener('click', cerrarSesion);
    $('reintentar').addEventListener('click', () => window.location.reload());
    for (const campo of [password, confirmacion]) {
      campo.addEventListener('input', () => confirmacion.setCustomValidity(''));
    }
    // iniciar gestiona sus propios errores; no hay promesas rechazadas sin gestionar.
    void iniciar();
  })();
  </script>
</body>
</html>
