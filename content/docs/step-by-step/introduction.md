+++
title = "Dependency Graph of things to do"
description = ""
date = 2021-05-01T08:00:00+00:00
updated = 2021-05-01T08:00:00+00:00
draft = false
weight = 10
sort_by = "weight"
template = "docs/page.html"

[extra]
lead = 'A dependency graph of things we needs to do.'
toc = true
top = false
+++

<pre class="mermaid">
    graph LR
        travel[<a href="/first-week-in-chalmers/docs/transport/ticket">Public transport tickets</a>] --> accommodation[Get accommodation keys]
        accommodation --> furniture[Buy Furnitures]
        accommodation --> internet[Internet Connection]
        accommodation --> cook[Use the kitchen]
        accommodation --> laundry[Use the laundry]
        accommodation --> rubbish[Throw rubbish]
        travel --> traffic[Travel hints]
        travel -.-> personal
        personal[<a href="/first-week-in-chalmers/docs/id/personal-number">Personal Number</a>] --> bank[Open Bank Account]
        travel -.-> Shopping
        DigitalStudentCard[Digital Student Card & Mercant]
        DigitalStudentCard --> PhysicalStudentCard[Physical Student Card]
        DigitalStudentCard -.-> travel
        phone[<a href="/first-week-in-chalmers/docs/phone/circ-sim/">Telephone number</a>]
        Refresh[Refresh residence permit]
        personal --> SFI[Swedish course For Immigrants]
        DigitalStudentCard -.-> bicycle[<a href="/first-week-in-chalmers/docs/transport/shared-bicycle/">Shared bicycle</a>]
        course[Register for courses and exams]
        timeEdit[Check time of your classes]
</pre>

<script type="module">
    import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
    mermaid.initialize({ startOnLoad: true });
</script>
