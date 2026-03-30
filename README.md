# 🎨 VOR-Bench: A Human Perception-Driven Benchmark for Video Object Removal
# 📖Introduction:
VOR-Bench is a novel and comprehensive benchmark designed to evaluate video object removal (VOR) quality, consisting of three core components: (1) VORD: The first evaluation dataset that provides both paired edited videos and graffiti masks. （2）rMPAP: A realistic Motion-capable Paired-video Acquisition Pipeline, based on the image removal model and video generation models. （3）VOR-MDSM: The first multi-dimensional scoring model aligned with human perception based on VLM models.
# 📅TODO：
- [x]  Release benchmark datasets.
- [ ]  Release VOR-MDSM's checkpoint.
- [ ]  Release VOR-MDSM's evalution code.
# 📂Dataset:
We propose VORD, the first evaluation dataset to simultaneously include video pairs (before and after removal) and graffiti masks. It consists of three types of video pairs including 🤖model-generated, 📸camera-captured, and 🛠️tool-rendered videos in equal proportions, covering 8 removal object types, 3 real-world scenarios, and 3 object association effects.
Furthermore, compared to traditional segmentation masks, we introduce graffiti masks that better align with authentic user input. Specifically, we use manually drawn masks for the first frame to simulate real user interactions, while using segmentation masks for the subsequent frames. VORD contains a total of 150 test cases, where each case includes the original video (rgb_full.mp4), the ground-truth video after removal (rgb_removed.mp4), and the graffiti mask video (mask_drawn.mp4). You can download this dataset via the [huggingface link🤗](https://huggingface.co/datasets/zangxh/VORD/tree/main).
# 🤝Acknowledgement:
Data Source: The tool-rendered videos in VORD are sourced from [ROSE-Bench](https://github.com/younglab/ROSE). We sincerely thank the authors for their high-quality work and for sharing these resources with the community.
Model Foundation: VOR-MDSM is built upon the [Qwen3-VL](https://github.com/QwenLM/Qwen3-VL) architecture. We appreciate the Qwen team for their contribution to the open-source community.


