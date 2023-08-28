+++
title = "不要急，一步步来"
description = ""
date = 2023-08-28T18:17:50.761Z
updated = 2023-08-28T18:17:50.761Z
draft = false
weight = 10
sort_by = "weight"
template = "docs/page.html"

[extra]
lead = '要做的事之间的依赖关系图'
toc = true
top = false
+++

实线代表**必须**做完之前的这件事才能做下一件事。

虚线代表**推荐**做完之前的这件事才能做下一件事，例如会有优惠之类的。

<pre class="mermaid">
    graph LR
        travel[<a href="/zh/docs/transport/ticket">买公共交通票</a>] --> accommodation[拿宿舍钥匙]
        accommodation --> furniture[买家具]
        accommodation --> internet[连上互联网]
        accommodation --> cook[用厨房]
        accommodation --> laundry[用洗衣房]
        accommodation --> rubbish[垃圾分类]
        accommodation --> shopping[快递服务]
        travel --> traffic[出行提示]
        travel -.-> personal
        personal[<a href="/zh/docs/id/personal-number">人口号</a>] --> bank[开银行账户]
        travel -.-> Shopping
        DigitalStudentCard[电子学生卡 & Mercant]
        DigitalStudentCard --> PhysicalStudentCard[实体学生卡]
        DigitalStudentCard -.-> travel
        phone[<a href="/zh/docs/phone/circ-sim/">手机号码</a>]
        Refresh[更新居留许可]
        personal --> SFI[Swedish course For Immigrants]
        DigitalStudentCard -.-> bicycle[<a href="/zh/docs/transport/shared-bicycle/">共享单车</a>]
        course[注册课程和考试]
        timeEdit[查看课程时间]
        doors[如何打开各个设施的大门]
</pre>

<script type="module">
    import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
    mermaid.initialize({ startOnLoad: true });
</script>
