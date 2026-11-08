# Welcome to the Single Board Cluster Competition 2027!

The *Single-Board Cluster Competition (SBCC)* is an international competition where teams build miniature supercomputing clusters using single-board computers and other similarly compact computing hardware.

SBCC27 marks the fifth edition of the competition.

This website provides information for participating teams, including competition regulations, hardware requirements, submissions, and logistical details. Additional information will be published as the competition approaches.

## FAQ <a id="faq"></a>

### What is the hardware budget?

The maximum hardware budget is **$6,000 USD**. International teams may use local market prices converted to USD. Used hardware is permitted with appropriate pricing documentation.

### What is the power limit?

The maximum total cluster power consumption is **300 W measured at the wall**, including compute nodes, networking equipment, storage, cooling, and all other peripherals.

Additionally, each processor or SoC package is subject to a **20 W TDP limit**.

### Are eGPUs allowed?

Yes, provided they comply with the hardware budget, processor eligibility requirements, and total wall-power limit.

### Does a DHCP server count as part of the cluster?

A separate DHCP server used solely for cluster network management is not considered a compute node. Its eligibility and power accounting are subject to competition regulations.

### Can we use LLMs during the competition?

Yes. LLMs may be used for assistance with development, debugging, and optimization. Competition workloads must still execute on the team's approved local cluster.

### Can we wirelessly access our cluster during the competition?

No. Cluster access must use wired connections unless the organizing committee explicitly authorizes an exception.

## Join Our Discord!

<script>
    document.addEventListener("DOMContentLoaded", function () {
        const mdContainer = document.querySelector("#mdbook-content > main");
        if (!mdContainer) return;

        const mediaQuery = window.matchMedia("(prefers-color-scheme: dark)");

        function createIframe(theme) {
            const iframe = document.createElement("iframe");
            iframe.src = `https://discord.com/widget?id=1462340210120720386&theme=${theme}`;
            iframe.setAttribute("allowtransparency", "true");
            iframe.setAttribute("frameborder", "0");
            iframe.setAttribute(
                "sandbox",
                "allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"
            );

            iframe.style.width = "50vw";
            iframe.style.height = "45vh";
            iframe.style.border = "0";

            return iframe;
        }

        let iframe = createIframe(mediaQuery.matches ? "dark" : "light");
        mdContainer.appendChild(iframe);

        mediaQuery.addEventListener("change", function (e) {
            const newTheme = e.matches ? "dark" : "light";
            const newIframe = createIframe(newTheme);
            iframe.replaceWith(newIframe);
            iframe = newIframe;
        });
    });
</script>