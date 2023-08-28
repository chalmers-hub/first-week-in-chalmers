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
        travel[<a href="/docs/transport/ticket">Public transport tickets</a>] --> accommodation[Get accommodation keys]
        accommodation --> furniture[Buy Furniture]
        accommodation --> internet[Internet Connection]
        accommodation --> cook[Use the kitchen]
        accommodation --> laundry[Use the laundry]
        accommodation --> rubbish[<a href="/docs/living/rubbish">Throw rubbish</a>]
        accommodation --> shopping[Online shopping delivery]
        travel --> traffic[Travel hints]
        travel -.-> personal
        personal[<a href="/docs/id/personal-number">Personal Number</a>] --> bank[Open Bank Account]
        travel -.-> Shopping
        DigitalStudentCard[Digital Student Card & Mercant]
        DigitalStudentCard --> PhysicalStudentCard[Physical Student Card]
        DigitalStudentCard -.-> travel
        phone[<a href="/docs/phone/circ-sim/">Telephone number</a>]
        Refresh[Refresh residence permit]
        personal --> SFI[Swedish course For Immigrants]
        DigitalStudentCard -.-> bicycle[<a href="/docs/transport/shared-bicycle/">Shared bicycle</a>]
        course[Register for courses and exams]
        timeEdit[Check time of your classes]
        doors[enter the facilities]
</pre>

<script type="module">
    import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
    mermaid.initialize({ startOnLoad: true });
</script>
