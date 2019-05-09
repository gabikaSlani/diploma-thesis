---
title: Diplomová práca
layout: default
---

<div class="container-fluid">
    <div class="row-fluid">
        <div class="col-md-8">
            <h3 class="title with-icon"><span class="fa fa-book cat-title"></span>Zadanie</h3>
                <ul class="timeline">
                    <li class="timeline-inverted">
                        <div class="timeline-badge info"></div>
                        <div class="timeline-panel grid-block">
                            <div class="timeline-heading">
                                <h4 class="timeline-title"><strong>Anotácia</strong></h4>
                            </div>
                            <div class="timeline-body">
                                <p>Existuje aplikácia imhd ba, ktorá slúži na plánovanie cesty v MHD v Bratislave na základe statických cestovných poriadkov. Cieľom tejto práce je nájsť spôsob určovania optimálnej cesty a naprogramovať aplikáciu, ktorá to dokáže urobiť z reálnych dát o pohybe vozidiel MHD.</p>
                            </div>
                        </div>
                    </li>
                </ul>
                <h3 class="title with-icon"><span class="fa fa-link cat-title"></span>Zdroje</h3>
                <ul class="timeline">
                    <li class="timeline-inverted">
                        <div class="timeline-badge info"></div>
                        <div class="timeline-panel grid-block">
                            <div class="timeline-heading">
                                <h4 class="timeline-title"><strong>Vedecké články</strong></h4>
                            </div>
                            <div class="timeline-body">
                                <p class="border"><a href="https://github.com/gabikaSlani/diploma-thesis/blob/master/articles/A_new_time-dependent_shortest_path_algorithm_for_multimodal_transportation_network.pdf">
                                  Abdelfattah Idri, Mariyem Oukarfi, Azedine Boulmakoul, Karine Zeitouni, and Ali Masri. <strong>A new time-dependent shortest path algorithm for multimodal transportation network.</strong> Procedia Computer Science, 109:692 - 697, 2017. 8th International Conference on Ambient Systems, Networks and Technologies, ANT-2017 and the 7th International Conference on Sustainable Energy Information Technology, SEIT 2017, 16-19 May 2017, Madeira, Portugal.
                                </a></p>
                                <p class="border"><a href="https://github.com/gabikaSlani/diploma-thesis/blob/master/articles/Shortest_alternate_path_discovery_through_recursive_bounding_box_pruning.pdf">
                                  R. Parmar and B. Trivedi. <strong>Shortest alternate path discovery through recursive bounding box pruning.</strong> Journal of Transportation Technologies, 7:167 - 180, 2017.
                                </a></p>
                                <p class="border"><a href="https://github.com/gabikaSlani/diploma-thesis/blob/master/articles/Optimal_route_computation_for_circilar_public_transport_routes_with_differential_fare_structure.pdf">
                                  Lilian S.C. Pun-Cheng and Albert W.F. Chan. <strong>Optimal route computation for circular public transport routes with differential fare structure.</strong> Travel Behaviour and Society, 3:71 - 77, 2016.
                                </a></p>
                                <p><a href="https://github.com/gabikaSlani/diploma-thesis/blob/master/articles/Towards_Online_Shortest_Paths_Computation.pdf">
                                  L. H. U, H. J. Zhao, M. L. Yiu, Y. Li, and Z. Gong. <strong>Towards online shortest path computation.</strong> IEEE Transactions on Knowledge and Data Engineering, 26(4):1012 - 1025, April 2014.
                                </a></p>
                            </div>
                        </div>
                    </li>
                </ul>
                <h3 class="title with-icon"><span class="fa fa-mobile fa-lg cat-title"></span>Prototyp</h3>
                <ul class="timeline">
                    <li class="timeline-inverted">
                        <div class="timeline-badge info"></div>
                        <div class="timeline-panel grid-block">
                            <div class="timeline-heading">
                                <h4 class="timeline-title"><strong>Android aplikácia A* algoritmus</strong></h4>
                            </div>
                            <div class="timeline-body">
                                <p>Aplikácia zobrazí statický ohodnotený graf a ponúkne používateľovi navoliť si začiatočný a koncový vrchol. Po zadaní vrcholov nájde pomocou A* algoritmu najkratšiu cestu.</p>
                                <p><a href="https://github.com/gabikaSlani/diploma-thesis/tree/master/code/shortestPathApp" target="_blank" class="link">
                                  GITHUB
                                </a></p>
                            </div>
                        </div>
                    </li>
                </ul>
                <h3 class="title with-icon"><span class="fa fa-file cat-title"></span>Dokumenty</h3>
                <ul class="timeline">
                    <li class="timeline-inverted">
                        <div class="timeline-badge info"></div>
                        <div class="timeline-panel grid-block">
                            <div class="timeline-heading">
                                <h4 class="timeline-title"><strong>Latex</strong></h4>
                            </div>
                            <div class="timeline-body">
                                <p><a href="https://github.com/gabikaSlani/diploma-thesis/blob/master/latex/main.pdf" class="link">
                                  PDF Dokument
                                </a></p>
                                <p><a href="https://github.com/gabikaSlani/diploma-thesis/blob/master/latex/literatura.bib" class="link">
                                  BibTex súbor
                                </a></p>
                            </div>
                        </div>
                    </li>
                    <li class="timeline-inverted">
                        <div class="timeline-badge info"></div>
                        <div class="timeline-panel grid-block">
                            <div class="timeline-heading">
                                <h4 class="timeline-title"><strong>Prezentácia</strong></h4>
                            </div>
                            <div class="timeline-body">
                                <p><a href="" class="link">
                                  PDF Dokument
                                </a></p>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        <div class="col-md-4">
            {% if site.author.stackoverflow or site.author.programmingSkills %}
                <h3 class="title with-icon"><span class="fa fa-line-chart cat-title"></span>Progres</h3>
                {% if site.author.stackoverflow %}
                <div class="grid-block">
                  <p><a href="//stackoverflow.com/users/{{ site.author.stackoverflow }}"><img src="//stackoverflow.com/users/flair/{{ site.author.stackoverflow }}.png"></a></p>
                  <ul class="list-unstyled list-stackoverflow" id="stackoverflow_questions_and_answers"></ul>
                  <script type="text/javascript">
                  $(function () {
                    var api_url_user = "//api.stackexchange.com/2.2/users/{{ site.author.stackoverflow }}/answers?pagesize=5&order=desc&sort=votes&site=stackoverflow";
                    var api_url_format_questions = "//api.stackexchange.com/2.2/questions/%question_ids%?site=stackoverflow";
                    $.get(api_url_user, function (data_user) {
                      if (!data_user) {
                        return;
                      }
                      if (!data_user.items) {
                        return;
                      }
                      if (!data_user.items.length) {
                        return;
                      }
                      var question_ids = [];
                      var complex_questions = {};
                      $.each(data_user.items, function (index, item) {
                        if (!item) {
                          return;
                        }
                        if (!item.question_id) {
                          return;
                        }
                        if (!item.answer_id) {
                          return;
                        }
                        if (!item.score) {
                          return;
                        }
                        complex_questions[item.question_id] = {
                          "question_id": item.question_id,
                          "answer_id": item.answer_id,
                          "score": humanize_score(item.score),
                          "is_accepted": item.is_accepted
                        };
                        question_ids.push(item.question_id);
                      });
                      var api_url_questions = api_url_format_questions.replace('%question_ids%', question_ids.join(';'));
                      $.get(api_url_questions, function (data_questions) {
                        if (!data_questions) {
                          return;
                        }
                        if (!data_questions.items) {
                          return;
                        }
                        if (!data_questions.items.length) {
                          return;
                        }
                        $.each(data_questions.items, function (index, item) {
                          if (!item) {
                            return;
                          }
                          if (!item.question_id) {
                            return;
                          }
                          var complex_question = complex_questions[item.question_id];
                          if (!complex_question) {
                            return;
                          }
                          complex_question.title = item.title;
                          complex_question.link = item.link;
                        });
                        render_complex_questions(complex_questions);
                      });
                    });
                  });
                  function humanize_score(score) {
                    if (!score) {
                      return;
                    }
                    if (score / 1000 > 1) {
                      return (score / 1000) + "k";
                    } else {
                      return score;
                    }
                  }
                  function render_complex_questions(complex_questions) {
                    if (!complex_questions) {
                      return;
                    }
                    complex_questions = $.map(complex_questions, function (complex_question) {
                      return [complex_question];
                    });
                    complex_questions.sort(function (a, b) {
                      return b.score - a.score;
                    });
                    $stackoverflow_questions_and_answers = $('#stackoverflow_questions_and_answers');
                    $.each(complex_questions, function (index, complex_question) {
                      var link = complex_question.link + '#answer-' + complex_question.answer_id;
                      var $li = $('<li />');
                      $('<span />')
                        .addClass('badge')
                        .addClass(complex_question.is_accepted ? 'progress-bar-success' : '')
                        .text(complex_question.score)
                        .appendTo($li);
                      $('<a />')
                        .attr('href', link)
                        .attr('target', '_blank')
                        .text(complex_question.title)
                        .appendTo($li);
                      $li.appendTo($stackoverflow_questions_and_answers);
                    });
                  }
                  </script>
                </div>
                {% endif %}
                {% if site.author.programmingSkills %}
                <div class="grid-block">
                    <ul class="list-unstyled list-skills">
                        {% for programmingSkill in site.author.programmingSkills %}
                            <li>
                                {% if programmingSkill.name %}
                                    <span class="caption-skill">{{ programmingSkill.name }}</span>
                                {% endif %}
                                {% if programmingSkill.percentage %}
                                    <div class="progress">
                                        <div class="progress-bar" style="width: {{ programmingSkill.percentage }}">
                                            <span>{{ programmingSkill.percentage }} </span>
                                        </div>
                                    </div>
                                {% endif %}
                            </li>
                        {% endfor %}
                    </ul>
                </div>
                {% endif %}
            {% endif %}
            <!-- {% if site.author.languages %}
                <div class="deviter"></div>
                <h3 class="title with-icon"><span class="fa fa-globe cat-title"></span> Language Skills</h3>
                <div class="grid-block">
                    <ul class="list-unstyled list-strip">
                        {% for language in site.author.languages %}
                            {% if language.name %}
                                {% if language.proficiency %}
                                    <li>
                                        <i class="fa fa-check"></i> <span class="badge badge-green badge-right-float">{{ language.proficiency }}</span>{{ language.name }}
                                    </li>
                                {% endif %}
                            {% endif %}
                        {% endfor %}
                    </ul>
                </div>
            {% endif %} -->
            <!-- <div class="deviter"></div>
            <h3 class="title with-icon"><span class="fa fa-location-arrow cat-title"></span> Location</h3>
            <div class="grid-block">
                <iframe src="https://www.google.com/maps/embed/v1/place?q={{ site.author.address }}&key=AIzaSyClEWLh20lxrQBFR7omuuVESviszPxONyk" width="100%" height="100%" frameborder="0" style="border:0"></iframe>
            </div> -->
        </div>
    </div>
</div>
