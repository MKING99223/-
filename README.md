AI Agent MVP
AI Agent MVP 是一个基于 Python 的本地可运行智能问答助手项目，利用 OpenAI 的 GPT 模型实现自然语言对话功能。该项目适合用作 AI Agent 原型、学习和演示用途，也可以作为后续扩展的基础架构。
核心功能


自然语言问答


用户可以在终端输入问题，AI Agent 基于 GPT 模型生成回答。




本地对话记录


每次问答会自动记录到 data/conversation_log.txt，便于追踪历史。




简单可扩展架构


项目使用模块化设计，agent_core.py 负责核心逻辑，utils.py 负责工具函数，可轻松扩展功能。




易于运行


只需安装依赖并设置 OpenAI API Key 即可快速启动。




轻量级


无需复杂部署，适合本地快速测试和开发。




技术栈


Python 3.8+


OpenAI Python SDK


python-dotenv 用于管理环境变量


项目结构
AI_Agent_MVP/│├── README.md├── requirements.txt├── main.py├── agent/│   ├── __init__.py│   ├── agent_core.py│   └── utils.py└── data/    └── conversation_log.txt
快速开始


安装依赖


pip install -r requirements.txt


设置 API Key
在项目根目录创建 .env 文件，并添加你的 OpenAI API Key：


OPENAI_API_KEY=你的OpenAI_API_Key


运行项目
python main.py
交互
在终端输入问题，AI Agent 会返回回答，输入 exit 或 quit 可退出程序。
