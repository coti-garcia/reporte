<template>
  <div
    class="testimonial-slider-area section-space--ptb_120 bg-gray"
    id="cartas"
  >
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            circleValue="02"
            class="section-space--mb_40"
            color="bodega"
            sectionProgress="20"
          />
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center section-space--mb_60">
            <h2 class="section-title font-width--light bodega">
              Cartas de presentación
            </h2>
          </div>
          <div class="testimonial-slider">
            <div class="swiper-container testimonial-slider__container">
              <div class="swiper-wrapper testimonial-slider__wrapper">
                <swiper :options="swiperOption">
                  <div class="swiper-slide">
                    <div class="testimonial-slider__one option-one">
                      <div class="row">
                        <div class="col-md-4">
                          <div class="testimonial-slider-side-info">
                  
                              <img
                                src="../assets/img/team/Mauricio-Canoles.jpg"
                                class="img-fluid"
                                alt=""
                              />
    
                            <div class="testimonial-slider__author">
                                                                <h6 class="bodega">  Este documento es una pausa en el camino para
                                    reflexionar sobre nuestros logros y forma de trabajo, de
                                    manera de seguir apoyando la innovación en la industria
                                    y la sociedad chilena</h6>
                              <h6 class="name bodega">Dr. Mauricio Cañoles</h6>
                              <div class="designation">Gerente General
                              </div>
                              <div class="designation">
                                  UC Davis Chile
                              </div>
                            </div>
                          </div>
                        </div>
                        <div class="col-md-4 text-carta">
                          <p>UC Davis Chile es uno de los Centros Excelencia Internacional que han sido invitados por el Estado de Chile a formar parte de un sistema de Investigación, Desarrollo e Innovación a través del Programa de Atracción impulsado por CORFO. El norte de nuestro Centro siempre ha estado claro: “brindar soluciones tecnológicas basadas en ciencia al mercado y a la sociedad”.</p>
                        <p>Fue a inicios del 2015 cuando nuestras actividades comienzan de forma “novedosa” en estrecha relación con la industria vitivinícola de nuestro país. Para esto un grupo multidisciplinario (estado, academia e industria) viajan a California para dar forma a nuestra primera hoja de ruta de trabajo técnico. Una “inmersión” en el trabajo de investigación que nuestra universidad en California, University of California Davis, estaba haciendo en ese entonces para apoyar el desarrollo de la viticultura y enología del estado. La biotecnología aplicada y la agricultura inteligente, aplicadas de forma metódica y sistemática para enfrentar desafíos reales de la industria Californiana, fueron las primeras ventanas de la relación Ciencia - Industria que se abren como un modelo a observar y adaptar cautelosamente desde Chile.
                            Esta ha sido una experiencia abierta a todos, parte o no del proyecto original, desde la industria hasta la academia, pasando por las instituciones del Estado.</p>
                        <p>Después de cinco años, casi seis, vemos como el quehacer de UC Davis Chile se ha basado en tres pilares fundamentales:
                          <ul>
                            <li>Estrecha colaboración con las instituciones de I+D chilenas</li>
                            <li>Incorporación activa de las empresas receptoras de las soluciones en nuestras actividades</li>
                            <li>Transferencia efectiva de la experiencia de nuestra Universidad, aciertos y errores, actuando como un puente tecnológico desde California a Chile.</li>
                          </ul>
                        </p>
                        </div>
                        <div class="col-md-4 text-carta">
                          <p>Si bien partimos con un modelo relativamente simple que asume un desarrollo de tecnología que es rápidamente incorporado por la industria, este es adaptado en nuestros primeros años para ajustarse a los requerimientos de Chile, su cultura, sus instituciones y sus necesidades y carencias. Desde la industria vitivinícola crecimos a un trabajo más amplio en Agricultura, Alimentos y Ambiente, iniciativas que son compartidas en este documento. Identificamos que la Adopción Tecnológica es un proceso lento que requiere más que sólo I+D, por lo que trabajamos fuertemente en fortalecer los procesos de Transferencia Tecnológica y Extensión, especialmente este último. Hemos crecido en nuestra red de colaboración tanto académica como empresarial y pública, lo que muestra nuestro tremendo compromiso con los socios estratégicos del centro.</p>
                        <p>Este documento es una recopilación de nuestras actividades en cinco años de vida en Chile. Pretende además mostrar con hechos y acciones la evolución de nuestro trabajo y convertirse en un hito de reflexión para nuestro trabajo futuro.</p>
                        <p>Los desafíos futuros, como siempre, requieren de un trabajo conjunto entre la academia, el sector público y la industria. Para esto UC Davis Chile sigue trabajando en compartir la experiencia de California y su red internacional fortaleciendo los procesos de I+D, Transferencia Tecnológica y Extensión. Esperamos que este documento sea una “muestra” de lo que podemos lograr en forma colaborativa para el desarrollo económico y social de Chile.</p>
                        </div>
                      </div>  
                    </div>
                  </div>
                  <div class="swiper-slide">
                    <div class="testimonial-slider__one option-one">
                      <div class="row">
                        <div class="col-md-4">
                          <div class="testimonial-slider-side-info">
                  
                              <img
                                src="../assets/img/team/Lovell_Tu_Jarvis.jpg"
                                class="img-fluid"
                                alt=""
                              />
    
                            <div class="testimonial-slider__author">
                                <h6 class="bodega">  Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo architecto enim fugiat placeat praesentium ratione necessitatibus ipsum repellendus nemo dicta sint.</h6>
                              <h6 class="name bodega">Lovell “Tu” Jarvis</h6>
                              <div class="designation">Director Ejecutivo
                              </div>
                              <div class="designation">
                                  UC Davis Chile
                              </div>
                            </div>
                          </div>
                        </div>
                        <div class="col-md-4 text-carta">
                          <p>La Universidad de California, Davis, es una de las grandes universidades públicas de Estados Unidos, dedicada a entregar una educación, investigación y servicio de primera a la sociedad.  UC Davis tiene una larga y fructífera trayectoria de colaboración con instituciones chilenas.  Por ejemplo, un gran número de científicos chilenos de las plantas estudiaron en UC Davis en los años sesenta.  Al regresar a Chile, estos científicos desempeñaron un papel clave en el desarrollo de la industria chilena de la fruta fresca, convirtiéndola en la potencia que es hoy.  Las conexiones que el sector agrícola chileno forjó con UC Davis en aquel momento siguen vigentes y hoy están cada vez más activas. </p>
                          <p>UC Davis creó el Centro de Innovación de las Ciencias de la Vida (también conocido como Centro UC Davis Chile) en 2014, con la asistencia de CORFO y con el fin de realizar investigaciones innovadoras y lograr la transferencia de tecnología en colaboración con socios académicos e industriales de Chile. El Centro facilita el acceso de los chilenos a la experiencia y los conocimientos de California, los cuales a menudo son muy relevantes para Chile debido a las muchas similitudes entre las dos regiones, por ejemplo, en términos de su geografía, clima, industrias, sociedad, y universidades.  A menudo los descubrimientos científicos y las nuevas tecnologías desarrolladas en California son aplicables a Chile con relativamente pocos ajustes, y viceversa.  Aprendemos y nos beneficiamos el uno del otro.  </p>
                          <p>El Centro UC Davis Chile busca soluciones que beneficien a los productores y consumidores de Chile a través de la creación de nuevas tecnologías y mejores políticas públicas. Trabajamos estrechamente con órganos del gobierno chileno y colaboramos con socios universitarios chilenos.   </p>
                        </div>
                        <div class="col-md-4 text-carta">
                          <p>Con un enfoque en la agricultura y el medio ambiente, el Centro ha contribuido al bienestar de Chile a través de muchos proyectos, como mejorar la genómica de las plantas, el control de enfermedades y la perfección de la gestión de riego en viñedos; el desarrollo de un programa de extensión exitoso para productores de vino pequeños y medianos, y la creación de un sitio de web de extensión integral del vino.  En otro proyecto, el Centro está desarrollando un sitio web público para informar a los usuarios sobre la disponibilidad de agua en una cuenca importante. En otro proyecto más estamos desarrollando modelos matemáticos para demostrar el impacto de los contaminantes y el cambio climático sobre la calidad del agua lacustre, entregando la información necesaria a los formuladores de políticas para diseñar políticas públicas que sostengan estos ambientes lacustres en el tiempo. </p>
                          <p>Más recientemente, trabajando con agencias gubernamentales adicionales y a través de mayores lazos con universidades chilenas, hemos ampliado las colaboraciones en áreas como la gestión de la calidad del aire, la infraestructura pública para apoyar la adopción de vehículos eléctricos y de hidrógeno, mayores beneficios de la telemedicina, la adopción de tecnología de iluminación mejorada, y el aumento de ahorros a través de un enfoque en la economía circular.  </p>
                          <p>El Centro UC Davis Chile está desarrollando colaboraciones académico-científicas que contribuyen al desarrollo económico y social de Chile.   Estamos encantados de estar en Chile.  Esperamos ampliar nuestras colaboraciones y contribuciones mutuamente beneficiosas en los próximos años.   </p>
                          <p>Sinceramente, <br />Lovell “Tu” Jarvis</p>
                        </div>
                      </div>  
                    </div>
                  </div>
                </swiper>
              </div>
            </div>
            <div
              class="swiper-pagination swiper-pagination-1 section-space--mt_60"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ChartCircleTwo from "../components/ChartCircleTwo";
import SectionTitle from "../components/SectionTitle";
export default {
  name: "Cartas",
  components: {
    ChartCircleTwo,
    SectionTitle,
  },
  data() {
    return {
      swiperOption: {
        speed: 800,
        loop: false,
        slidesPerView: 1,
        spaceBetween: 30,
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.option-two {
  .testimonial-slider__text {
    color: #333;
    column-count: 2;
    column-gap: 60px;
    p {
      font-size: 16px;
    }
    @media #{$large-mobile} {
      column-count: 1;
    }
  }
}
.option-one {
  .text-carta {
    margin-top: 80px;
  }
  .testimonial-slider__author {
    padding-left: 30%;
    h6 {
      font-weight: 600;
      font-size: 16px;
      padding-top: 20px;
      line-height: 1.3;
    }
  }
}

.post-thumbnail {
  .img-fluid {
    max-width: 100px;
    border-radius: 50%;
  }
}
.testimonial-slider__author {
  margin-top: 15px;
  .name {
    font-weight: 600;
  }
  .designation {
    color: #666666;
    font-size: 14px;
  }
}
ul {
  list-style: disc;
  padding-left: 20px;
}
</style>