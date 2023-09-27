---
title: About
layout: page
permalink: /about/
published: true
---

My name is Shinwoo Kim, and I am a BS+MS student at the [University of Pittsburgh](https://pitt.edu)'s [School of Computing and Information](https://sci.pitt.edu) studying Computer Science and Mathematics. My current interests are in the field of **computer systems, Operating systems, and computer architecture**, although there are very few things in computer science that I'm *not* interested in. Currently, I work as a [teaching assistant]({{ '/teaching/' | prepend: site.baseurl }}) for Pitt's Computer Science Department where I love trying new techniques to help students learn. Additionally, I also am the Lead Software Developer for the [*TouchTheInvisible*](https://touchtheinvisible.com) project at the University of Pittsburgh.

Previously, I worked as the STEAM ambassador[^sponser] at Pitt's [Hill District Community Engagement Center](https://cec.pitt.edu/hilldistrict/) where I taught K-12/young adult students about computer science and information technology. I was also a founding member of the [Special Needs Acceptance Project](https://snapfse.com/), a Pittsburgh organization which promotes the awareness of Neurodiverse[^neurodiverse] communities, and served on the inaugural advisory board.<span class="endmark"></span>

[^sponser]: Sponsored and funded by the [David C. Frederick Honors College](https://www.frederickhonors.pitt.edu/)
[^neurodiverse]: N. Baumer and J. Frueh, “What is neurodiversity?,” Harvard Health Publishing, [https://www.health.harvard.edu/blog/what-is-neurodiversity-202111232645](https://www.health.harvard.edu/blog/what-is-neurodiversity-202111232645)

## Education
<span class="h3"><i class="fa-solid fa-graduation-cap"></i>Master of Science, Computer Science, (Exp.) 2025</span>
{: .mb-0}

- <i class="pitt-icon"></i>University of Pittsburgh
  - School of Computing and Information

<span class="h3"><i class="fa-solid fa-graduation-cap"></i>Bachelor of Science, Computer Science, (Exp.) 2024</span>
{: .mb-0}

- <i class="pitt-icon"></i>University of Pittsburgh
  - School of Computing and Information
  - David C. Frederick Honors College

## Work Experiences

<div class="accordion accordion-flush border mb-0" id="accordionExperiences">
  <div class="accordion-item">
    <div class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
        data-bs-target="#currentPositions" aria-expanded="false" aria-controls="currentPositions">
        <div class="fw-bold h4">Current Positions</div>
      </button>
    </div>
    <div id="currentPositions" class="accordion-collapse collapse" aria-labelledby="currentPositions">
      <div class="accordion-body">
        <div class="accordion accordion-flush mb-0" id="currPos">
          {% for item in site.data.experiences.current %}
          <div class="accordion-item accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
              data-bs-target="#collapse{{item.id}}" aria-expanded="false" aria-controls="collapse{{item.id}}">
              <div class="h5">{{item.title}}</div>
            </button>
          </div>
          <div id="collapse{{item.id}}" class="accordion-collapse collapse" aria-labelledby="Acc_{{item.id}}">
            <div class="accordion-body">
              <div class="d-flex flex-column justify-content-between mb-3">
                <div class="d-md-flex justify-content-between mb-3">
                  <div class="flex-grow-1">
                    <p class="h5 mb-1">
                      <strong markdown="1">{{item.employer}}</strong>
                    </p>
                  </div>
                  <div class="flex-shrink-0">
                    <span class="text-pr  imary">{{item.duration}}</span>
                  </div>
                </div>
                <p class="mb-0 fs-6" markdown="1">{{item.desc}}</p>
              </div>
            </div>
          </div>
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <div class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
        data-bs-target="#previousPositions" aria-expanded="false" aria-controls="previousPositions">
        <div class="fw-bold h4">Previous Positions</div>
      </button>
    </div>
    <div id="previousPositions" class="accordion-collapse collapse" aria-labelledby="previousPositions">
      <div class="accordion-body">
        <div class="accordion accordion-flush mb-0" id="prevPos">
          {% for item in site.data.experiences.past %}
          <div class="accordion-item accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
              data-bs-target="#collapse{{item.id}}" aria-expanded="false" aria-controls="collapse{{item.id}}">
              <div class="h5">{{item.title}}</div>
            </button>
          </div>
          <div id="collapse{{item.id}}" class="accordion-collapse collapse" aria-labelledby="Acc_{{item.id}}">
            <div class="accordion-body">
              <div class="d-flex flex-column justify-content-between mb-3">
                <div class="d-md-flex justify-content-between mb-3">
                  <div class="flex-grow-1">
                    <p class="h5 mb-1">
                      <strong markdown="1">{{item.employer}}</strong>
                    </p>
                  </div>
                  <div class="flex-shrink-0">
                    <span class="text-primary">{{item.duration}}</span>
                  </div>
                </div>
                <p class="mb-0 fs-6" markdown="1">{{item.desc}}</p>
              </div>
            </div>
          </div>
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</div>
Please visit my [LinkedIn](https://linkedin.com/in/kimshinwoo) for the most up-to-date information.
{: .text-center .mt-3}

{% include icons.html %}

<style>ul{list-style: none;}</style>

---