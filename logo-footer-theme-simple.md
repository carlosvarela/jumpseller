 // Add this html code in your footer file footer.liquid around line 100
```
    
         <a href="{{store.url}}" title="{{store.name}}" class="brand-footer">
          {% if options.logo_footer != empty %}
          <img src="{{options.logo_footer | resize:'150'}}" class="store-image" alt="{{store.name}}" />
          {% else %}
          <h1><span class="text-logo">{{store.name}}</span></h1>
          {% endif %}
        </a>
  ```
      
        
// Add this snippet to your options.json
```
  
   "logo_footer": {
        "name": "Logo Pie de Página",
        "type": "file",
        "default": "",
        "help": "Tamaño recomendado 250 pixeles de ancho"
      },
        
// full version or if you want to replace options.json

{
  "General": {
    "icon": "cog",
    "options": {
      "favicon": {
        "name": "Favicon (Icono del Navegador)",
        "type": "file",
        "default": "",
        "help": ""
      },
      "logo_footer": {
        "name": "Logo Pie de Página",
        "type": "file",
        "default": "",
        "help": "Tamaño recomendado 250 pixeles de ancho"
      },
      "success_page_product_table": {
        "name": "Tabla de Productos en la Página de Éxito",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "hide_category_menu": {
        "name": "Ocultar Menú de Categorías",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "fetured_on_search": {
        "name": "Mostrar productos destacados cuando no hay resulta",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "products_category_limit": {
        "name": "Productos por Página en Categorías",
        "type": "select",
        "default": "12",
        "help": "",
        "options": [
          {
            "4": "4"
          },
          {
            "8": "8"
          },
          {
            "12": "12"
          },
          {
            "16": "16"
          },
          {
            "20": "20"
          },
          {
            "24": "24"
          },
          {
            "28": "28"
          },
          {
            "32": "32"
          },
          {
            "36": "36"
          },
          {
            "40": "40"
          }
        ]
      },
      "products_search_limit": {
        "name": "Productos por Página en el Resultado de Búsqueda",
        "type": "select",
        "default": "12",
        "help": "",
        "options": [
          {
            "4": "4"
          },
          {
            "8": "8"
          },
          {
            "12": "12"
          },
          {
            "16": "16"
          },
          {
            "20": "20"
          },
          {
            "24": "24"
          },
          {
            "28": "28"
          },
          {
            "32": "32"
          },
          {
            "36": "36"
          },
          {
            "40": "40"
          }
        ]
      },
      "page_post_per_page": {
        "name": "Publicaciones de Blog por Página",
        "type": "select",
        "default": "9",
        "help": "",
        "options": [
          {
            "6": "6"
          },
          {
            "9": "9"
          },
          {
            "12": "12"
          },
          {
            "15": "15"
          },
          {
            "18": "18"
          },
          {
            "21": "21"
          },
          {
            "24": "24"
          },
          {
            "27": "27"
          },
          {
            "30": "30"
          },
          {
            "33": "33"
          }
        ]
      }
    }
  },
  "Información de la Tienda": {
    "icon": "store",
    "options": {
      "display_contact_email": {
        "name": "Mostrar Email de Contacto Principal",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "phone": {
        "name": "Teléfono de Contacto Principal",
        "type": "input",
        "default": "",
        "help": ""
      },
      "working_hours": {
        "name": "Horarios de Trabajo de Tienda Principal",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_2_name": {
        "name": "Nombre de Tienda 2",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_2_address": {
        "name": "Dirección de Tienda 2",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_2_phone": {
        "name": "Teléfono de Tienda 2",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_2_hours": {
        "name": "Horarios de Trabajo de Tienda 2",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_3_name": {
        "name": "Nombre de Tienda 3",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_3_address": {
        "name": "Dirección de Tienda 3",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_3_phone": {
        "name": "Teléfono de Tienda 3",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_3_hours": {
        "name": "Horarios de Trabajo de Tienda 3",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_4_name": {
        "name": "Nombre de Tienda 4",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_4_address": {
        "name": "Dirección de Tienda 4",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_4_phone": {
        "name": "Teléfono de Tienda 4",
        "type": "input",
        "default": "",
        "help": ""
      },
      "store_4_hours": {
        "name": "Horarios de Trabajo de Tienda 4",
        "type": "input",
        "default": "",
        "help": ""
      }
    }
  },
  "Bloque de Producto": {
    "icon": "archive",
    "options": {
      "show_add_to_cart": {
        "name": "Mostrar Botón de Agregar al Carro",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "show_brand": {
        "name": "Mostrar Marca del Producto",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "from-prices": {
        "name": "Mostrar 'desde' en Precios de Productos con Varian",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "sale_tag": {
        "name": "Color de la etiqueta de promociones",
        "type": "color",
        "default": "f44336",
        "help": ""
      }
    }
  },
  "Página del Producto": {
    "icon": "archive",
    "options": {
      "product_stock_visibility": {
        "name": "Mostrar Stock del Producto",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "product_sku_visibility": {
        "name": "Mostrar SKU del Producto",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "related_products_visibility": {
        "name": "Mostrar Productos Relacionados",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "related_products_limit": {
        "name": "Cantidad Máxima de Productos Relacionados",
        "type": "select",
        "default": "8",
        "help": "",
        "options": [
          {
            "8": "8"
          },
          {
            "12": "12"
          },
          {
            "16": "16"
          },
          {
            "20": "20"
          },
          {
            "24": "24"
          },
          {
            "28": "28"
          },
          {
            "32": "32"
          },
          {
            "36": "36"
          },
          {
            "40": "40"
          }
        ]
      },
      "thumbnails_visibility": {
        "name": "Mostrar Miniaturas de Imágenes del Producto",
        "type": "checkbox",
        "default": "1",
        "help": ""
      }
    }
  },
  "Colores": {
    "icon": "tint",
    "options": {
      "general_text_color": {
        "name": "Color General del Texto",
        "type": "color",
        "default": "rgb(8,8,8,1)",
        "help": ""
      },
      "general_links_color": {
        "name": "Color General de los Enlaces",
        "type": "color",
        "default": "1e3b51",
        "help": ""
      },
      "primary_color": {
        "name": "Color Primario",
        "type": "color",
        "default": "rgb(117,110,13,1)",
        "help": ""
      },
      "secondary_color": {
        "name": "Color Secundario",
        "type": "color",
        "default": "rgb(46,74,10,1)",
        "help": ""
      },
      "store_background": {
        "name": "Fondo de la Tienda",
        "type": "color",
        "default": "rgb(255,255,255,1)",
        "help": ""
      }
    }
  },
  "Tipos de Letra": {
    "icon": "font",
    "options": {
      "general_font": {
        "name": "General",
        "type": "google_font",
        "default": "Open Sans",
        "help": "",
        "options": [
          {
            "Droid Serif": "Droid Serif"
          },
          {
            "Gentium Basic": "Gentium Basic"
          },
          {
            "Lato": "Lato"
          },
          {
            "Noto Sans": "Noto Sans"
          },
          {
            "Open Sans (by Default)": "Open Sans"
          },
          {
            "Playfair Display": "Playfair Display"
          },
          {
            "Quicksand": "Quicksand"
          },
          {
            "Raleway": "Raleway"
          },
          {
            "Roboto": "Roboto"
          },
          {
            "Roboto Slab": "Roboto Slab"
          }
        ]
      },
      "titles_font": {
        "name": "Títulos",
        "type": "google_font",
        "default": "Open Sans",
        "help": "",
        "options": [
          {
            "Abril Fatface": "Abril Fatface"
          },
          {
            "Architects Daughter": "Architects Daughter"
          },
          {
            "Fredericka the Great": "Fredericka the Great"
          },
          {
            "Glegoo": "Glegoo"
          },
          {
            "Handlee": "Handlee"
          },
          {
            "Josefin Slab": "Josefin Slab"
          },
          {
            "Julius Sans One": "Julius Sans One"
          },
          {
            "Lato": "Lato"
          },
          {
            "Libre Baskerville": "Libre Baskerville"
          },
          {
            "Montserrat": "Montserrat"
          },
          {
            "Open Sans (by Default)": "Open Sans"
          },
          {
            "Philosopher": "Philosopher"
          },
          {
            "Poiret One": "Poiret One"
          },
          {
            "Roboto": "Roboto"
          },
          {
            "Special Elite": "Special Elite"
          }
        ]
      },
      "store_name_font": {
        "name": "Nombre de la Tienda",
        "type": "google_font",
        "default": "Open Sans",
        "help": "",
        "options": [
          {
            "Abril Fatface": "Abril Fatface"
          },
          {
            "Architects Daughter": "Architects Daughter"
          },
          {
            "Fredericka the Great": "Fredericka the Great"
          },
          {
            "Libre Baskerville": "Libre Baskerville"
          },
          {
            "Open Sans (by Default)": "Open Sans"
          },
          {
            "Playfair Display": "Playfair Display"
          },
          {
            "Poiret One": "Poiret One"
          },
          {
            "Raleway": "Raleway"
          },
          {
            "Roboto": "Roboto"
          },
          {
            "Old Standard TT": "Old Standard TT"
          },
          {
            "Yatra One": "Yatra One"
          }
        ]
      },
      "general_font_size": {
        "name": "Tamaño de Letra General",
        "type": "select",
        "default": "16px",
        "help": "",
        "options": [
          {
            "10px": "10px"
          },
          {
            "11px": "11px"
          },
          {
            "12px": "12px"
          },
          {
            "13px": "13px"
          },
          {
            "14px (by Default)": "14px"
          },
          {
            "15px": "15px"
          },
          {
            "16px": "16px"
          },
          {
            "17px": "17px"
          },
          {
            "18px": "18px"
          }
        ]
      },
      "block_title_font_size": {
        "name": "Tamaño de Letra de Bloques de Título",
        "type": "select",
        "default": "20px",
        "help": "",
        "options": [
          {
            "12px": "12px"
          },
          {
            "14px": "14px"
          },
          {
            "16px": "16px"
          },
          {
            "18px (by Default)": "18px"
          },
          {
            "20px": "20px"
          },
          {
            "22px": "22px"
          },
          {
            "24px": "24px"
          },
          {
            "26px": "26px"
          },
          {
            "28px": "28px"
          },
          {
            "30px": "30px"
          }
        ]
      },
      "store_name_font_size": {
        "name": "Tamaño de Letra en Nombre de la Tienda ",
        "type": "select",
        "default": "20px",
        "help": "",
        "options": [
          {
            "14px": "14px"
          },
          {
            "15px": "15px"
          },
          {
            "16px": "16px"
          },
          {
            "17px": "17px"
          },
          {
            "18px (by Default)": "18px"
          },
          {
            "20px": "20px"
          },
          {
            "22px": "22px"
          },
          {
            "24px": "24px"
          },
          {
            "26px": "26px"
          },
          {
            "28px": "28px"
          },
          {
            "30px": "30px"
          },
          {
            "32px": "32px"
          },
          {
            "34px": "34px"
          },
          {
            "36px": "36px"
          },
          {
            "38px": "38px"
          },
          {
            "40px": "40px"
          }
        ]
      },
      "menu_font_size": {
        "name": "Tamaño de Letra del Menú",
        "type": "select",
        "default": "16px",
        "help": "",
        "options": [
          {
            "10px": "10px"
          },
          {
            "11px": "11px"
          },
          {
            "12px": "12px"
          },
          {
            "13px": "13px"
          },
          {
            "14px (by Default)": "14px"
          },
          {
            "15px": "15px"
          },
          {
            "16px": "16px"
          },
          {
            "17px": "17px"
          },
          {
            "18px": "18px"
          },
          {
            "20px": "20px"
          }
        ]
      }
    }
  },
  "Redes Sociales": {
    "icon": "share-alt",
    "options": {
      "facebook_button_on_products": {
        "name": "Botón de Facebook en Productos",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "twitter_button_on_products": {
        "name": "Botón de Twitter en Productos",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "pinterest_button_on_products": {
        "name": "Botón de Pinterest en Productos",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "tumblr_button_on_products": {
        "name": "Botón de Tumblr en productos",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "whatsapp_button_on_products": {
        "name": "Botón de WhatsApp en Productos en Móvil",
        "type": "checkbox",
        "default": "1",
        "help": ""
      }
    }
  },
  "Preguntas Frecuentes de la Tienda": {
    "icon": "question-circle",
    "options": {
      "faq": {
        "name": "Activar Preguntar Frecuentes",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "faq_title_1": {
        "name": "Título de Pregunta Frecuente 1",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número uno",
        "help": ""
      },
      "faq_answer_1": {
        "name": "Repuesta de Pregunta Frecuente 1",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_2": {
        "name": "Título de Pregunta Frecuente 2",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número dos",
        "help": ""
      },
      "faq_answer_2": {
        "name": "Repuesta de Pregunta Frecuente 2",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_3": {
        "name": "Título de Pregunta Frecuente 3",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número tres",
        "help": ""
      },
      "faq_answer_3": {
        "name": "Repuesta de Pregunta Frecuente 3",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_4": {
        "name": "Título de Pregunta Frecuente 4",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número cuatro",
        "help": ""
      },
      "faq_answer_4": {
        "name": "Repuesta de Pregunta Frecuente 4",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_5": {
        "name": "Título de Pregunta Frecuente 5",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número cinco",
        "help": ""
      },
      "faq_answer_5": {
        "name": "Repuesta de Pregunta Frecuente 5",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_6": {
        "name": "Título de Pregunta Frecuente 6",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número seis",
        "help": ""
      },
      "faq_answer_6": {
        "name": "Repuesta de Pregunta Frecuente 6",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_7": {
        "name": "Título de Pregunta Frecuente 7",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número siete",
        "help": ""
      },
      "faq_answer_7": {
        "name": "Repuesta de Pregunta Frecuente 7",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_8": {
        "name": "Título de Pregunta Frecuente 8",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número ocho",
        "help": ""
      },
      "faq_answer_8": {
        "name": "Repuesta de Pregunta Frecuente 8",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_9": {
        "name": "Título de Pregunta Frecuente 9",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número nueve",
        "help": ""
      },
      "faq_answer_9": {
        "name": "Repuesta de Pregunta Frecuente 9",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      },
      "faq_title_10": {
        "name": "Título de Pregunta Frecuente 10",
        "type": "input",
        "default": "Ejemplo de pregunta frecuente número diez",
        "help": ""
      },
      "faq_answer_10": {
        "name": "Repuesta de Pregunta Frecuente 10",
        "type": "text",
        "default": "Maecenas consequat nisl sit amet ante dictum ultricies. Sed efficitur sit amet sem quis finibus. Vestibulum ultrices arcu eu sapien bibendum malesuada in id justo. In massa ipsum, aliquet quis sagittis nec, euismod quis nunc. Maecenas vestibulum porta diam, nec commodo libero laoreet volutpat. Nam quis ipsum finibus, ultrices augue non",
        "help": ""
      }
    }
  },
  "Pie de Página": {
    "icon": "ellipsis-h",
    "options": {
      "enable_subscribe": {
        "name": "Habilitar Formulario de Suscripción",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "mailchimp_post_url": {
        "name": "Url del Formulario de Mailchimp",
        "type": "input",
        "default": "",
        "help": ""
      },
      "subscribe_title": {
        "name": "Título del Formulario",
        "type": "text",
        "default": "Suscríbete a nuestra lista de correo electrónico para recibir noticias y Ofertas primero.",
        "help": ""
      },
      "footer_color": {
        "name": "Color Footer",
        "type": "color",
        "default": "rgb(45,48,49,1)",
        "help": ""
      },
      "footer_link_color": {
        "name": "Color links",
        "type": "color",
        "default": "rgb(255,255,255,1)",
        "help": ""
      }
    }
  },
  "Métodos de pago para mostrar": {
    "icon": "credit-card",
    "options": {
      "webpay_payment": {
        "name": "Mostrar pago con Webpay",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "chek_payment": {
        "name": "Mostrar pago con Chek",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "khipu_payment": {
        "name": "Mostrar pago con Khipu",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "servipag_payment": {
        "name": "Mostrar pago con Servipag",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "mach_payment": {
        "name": "Mostrar pago con Mach",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "flow_payment": {
        "name": "Mostrar pago con Flow",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "caja_vecina_payment": {
        "name": "Mostrar pago con Caja Vecina",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "multicaja_payment": {
        "name": "Mostrar pago con Multicaja",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "pse_payment": {
        "name": "Mostrar pago con PSE ",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "baloto_payment": {
        "name": "Mostrar pago con Baloto",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "epayco_payment": {
        "name": "Mostrar pago con ePayco",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "efecty_payment": {
        "name": "Mostrar pago con Efecty",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "oxxo_payment": {
        "name": "Mostrar pago con Oxxo",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "mercadopago_payment": {
        "name": "Mostrar pago con Mercadopago",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "multibanco_payment": {
        "name": "Mostrar pago con Multibanco",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "mbway_payment": {
        "name": "Mostrar pago con MBWay",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "payu_payment": {
        "name": "Mostrar pago con PayU",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "ideal_payment": {
        "name": "Mostrar pago con iDEAL",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "skrill_payment": {
        "name": "Mostrar pago con Skrill",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "stripe_payment": {
        "name": "Mostrar pago con Stripe",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "apple_payment": {
        "name": "Mostrar pago con Apple Pay",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "bitcoin_payment": {
        "name": "Mostrar pago con Bitcoin",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "visa_payment": {
        "name": "Mostrar pago con Visa",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "mastercard_payment": {
        "name": "Mostrar pago con MasterCard",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "american_payment": {
        "name": "Mostrar pago con American Express",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "paypal_payment": {
        "name": "Mostrar pago con Paypal",
        "type": "checkbox",
        "default": "1",
        "help": ""
      },
      "diners_payment": {
        "name": "Mostrar pago con Diners Club",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "bank_transfer_payment": {
        "name": "Mostrar pago con Transferencia Bancaria",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "manual_payment": {
        "name": "Mostrar Pago Manual",
        "type": "checkbox",
        "default": "0",
        "help": ""
      }
    }
  },
  "Notificación de Agregar al Carro": {
    "icon": "shopping-cart",
    "options": {
      "display_cart_notification": {
        "name": "Notificación de Agregar al Carro",
        "type": "checkbox",
        "default": "1",
        "help": "La Notificación de Agregar al Carro sólo funciona cuando se selecciona la opción 'Seguir en la misma página' en 'Checkout > Configuración > Después de agregar un producto al carrito'."
      },
      "cart_notification_color": {
        "name": "Color de la Notificación",
        "type": "color",
        "default": "10e039",
        "help": ""
      },
      "cart_notification_position": {
        "name": "Posición",
        "type": "select",
        "default": "toast-top-right",
        "help": "",
        "options": [
          {
            "Top right": "toast-top-right"
          },
          {
            "Top left": "toast-top-left"
          },
          {
            "Bottom right": "toast-bottom-right"
          },
          {
            "Bottom left": "toast-bottom-right"
          }
        ]
      }
    }
  },
  "Otras Opciones": {
    "icon": "cogs",
    "options": {
      "new_customer_message": {
        "name": "Mensaje de Nuevo Cliente",
        "type": "text",
        "default": "Al registrarse en nuestra tienda, agilizará el proceso de pago, podrá agregar varias direcciones de envío, ver y rastrear sus pedidos y más.",
        "help": ""
      },
      "currencies": {
        "name": "Monedas adicionales (ej. USD, EUR)",
        "type": "input",
        "default": "",
        "help": ""
      },
      "open_exchange_rates_token": {
        "name": "ID de Aplicación OpenExchangeRates",
        "type": "input",
        "default": "",
        "help": ""
      },
      "preheader_message": {
        "name": "Mensaje promocional",
        "type": "input",
        "default": "Envío en 48 hrs en la V Región - Pedidos al +569 38643262 o a renato.caro.v@gmail.com",
        "help": ""
      },
      "disable_shopping_cart": {
        "name": "Deshabilitar Carro de Compras",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "hide_price": {
        "name": "Ocultar Precios",
        "type": "checkbox",
        "default": "0",
        "help": ""
      },
      "head_code": {
        "name": "Insertar código al final de <head>",
        "type": "text",
        "default": "",
        "help": ""
      },
      "body_code": {
        "name": "Insertar código al final de <body>",
        "type": "text",
        "default": "",
        "help": ""
      }
    }
  }
}
```
