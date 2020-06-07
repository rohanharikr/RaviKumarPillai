---
layout: page
title: Consulting
comments: false
---

<div class="wrapper">
  <h3>Strategy & Organization</h3>
  <div class="accordion">
    <div class="accordion-item">
      <button id="accordion-button-1" aria-expanded="false"><span class="accordion-title">Business & Operating Model</span><span class="icon" aria-hidden="true"></span></button>
      <div class="accordion-content">
        <p>Business Effectiveness<br> Audit : Review and alignment of structure, systems and competencies</p>
      </div>
    </div>
    <div class="accordion-item">
      <button id="accordion-button-2" aria-expanded="false"><span class="accordion-title">Total Rewards Management</span><span class="icon" aria-hidden="true"></span></button>
      <div class="accordion-content">
        <p>Salary Design, Job Evaluation, Market Pricing, Incentives Design, Stock Option;  Talent Retention Programs</p>
      </div>
    </div>
    <div class="accordion-item">
      <button id="accordion-button-3" aria-expanded="false"><span class="accordion-title">Business Transformation &  Change Management</span><span class="icon" aria-hidden="true"></span></button>
      <div class="accordion-content">
        <p>Comprehensive diagnosis and intervention program to drive corporate change</p>
      </div>
    </div>
  </div>
</div>
<div class="wrapper wrappertwo">
  <h3>Coaching and Mentoring</h3>
  <div class="accordion">
    <div class="accordion-item">
      <button id="accordion-button-1" aria-expanded="false"><span class="accordion-title">Competency Profiling & Assessment</span><span class="icon" aria-hidden="true"></span></button>
      <div class="accordion-content">
        <p>Customized competency  assessment and Individual Development Program</p>
      </div>
    </div>
    <div class="accordion-item">
      <button id="accordion-button-2" aria-expanded="false"><span class="accordion-title">Behaviour-anchored leadership coaching</span><span class="icon" aria-hidden="true"></span></button>
      <div class="accordion-content">
        <p>Design and delivery of intensive executive coaching </p>
      </div>
    </div>
  </div>
  <h3 id="contactme"><a href="{{ site.baseurl }}/contact">Contact Me</a></h3>
</div>




<script>
 const items = document.querySelectorAll(".accordion button");

function toggleAccordion() {
  const itemToggle = this.getAttribute('aria-expanded');
  
  for (i = 0; i < items.length; i++) {
    items[i].setAttribute('aria-expanded', 'false');
  }
  
  if (itemToggle == 'false') {
    this.setAttribute('aria-expanded', 'true');
  }
}

items.forEach(item => item.addEventListener('click', toggleAccordion));

</script>



  <style>

  	#contactme{
  		margin-top: 40px;
  	}

.wrapper {
  margin: 0 auto;
  padding: 4rem;
  width: 48rem;
  padding-bottom: 2em;
  padding-top: 2em;
}

.wrappertwo {
 padding: 0.3em 4rem; 
}

.accordion .accordion-item {
  border-bottom: 1px solid #e5e5e5;
}
.accordion .accordion-item button[aria-expanded='true'] {
  border-bottom: 1px solid #03b5d2;
}
.accordion button {
  position: relative;
  display: block;
  text-align: left;
  width: 100%;
  padding: 1em 0;
  color: #7288a2;
  font-size: 1.15rem;
  font-weight: 400;
  border: none;
  background: none;
  outline: none;
}
.accordion button:hover, .accordion button:focus {
  cursor: pointer;
  color: #03b5d2;
}
.accordion button:hover::after, .accordion button:focus::after {
  cursor: pointer;
  color: #03b5d2;
  border: 1px solid #03b5d2;
}
.accordion button .accordion-title {
  padding: 1em 1.5em 1em 0;
}
.accordion button .icon {
  display: inline-block;
  position: absolute;
  top: 18px;
  right: 0;
  width: 22px;
  height: 22px;
  border: 1px solid;
  border-radius: 22px;
}
.accordion button .icon::before {
  display: block;
  position: absolute;
  content: '';
  top: 9px;
  left: 5px;
  width: 10px;
  height: 2px;
  background: currentColor;
}
.accordion button .icon::after {
  display: block;
  position: absolute;
  content: '';
  top: 5px;
  left: 9px;
  width: 2px;
  height: 10px;
  background: currentColor;
}
.accordion button[aria-expanded='true'] {
  color: #03b5d2;
}
.accordion button[aria-expanded='true'] .icon::after {
  width: 0;
}
.accordion button[aria-expanded='true'] + .accordion-content {
  opacity: 1;
  max-height: 9em;
  -webkit-transition: all 200ms linear;
  transition: all 200ms linear;
  will-change: opacity, max-height;
}
.accordion .accordion-content {
  opacity: 0;
  max-height: 0;
  overflow: hidden;
  -webkit-transition: opacity 200ms linear, max-height 200ms linear;
  transition: opacity 200ms linear, max-height 200ms linear;
  will-change: opacity, max-height;
}
.accordion .accordion-content p {
  font-size: 1rem;
  font-weight: 300;
  margin: 2em 0;
}

  </style>


