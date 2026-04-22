# BLYe个人DJ工作室 - 智能音乐制作平台

## 项目概述
BLYe个人DJ工作室是一款专业的AI智能音乐制作平台，提供从音乐创作、编辑到导出的一站式服务。

## 核心功能

### 1. AI音乐生成
- 支持生成抖音热门DJ风格音乐
- 全中文歌词创作
- 自动编曲、混音
- 流式生成，实时预览

### 2. 音频分析与处理
- 上传歌曲自动分析
- 和弦、根音识别
- MIDI工程文件提取
- 人声、伴奏、贝斯等音轨分离
- 音频参数可视化

### 3. 变声器与音色调节
- 实时变声调节
- 音高调整（高/低）
- 性别转换
- 音色克隆训练
- 多种预设音色

### 4. 工程文件导出
- WAV/MP3/FLAC多格式支持
- 分轨导出（人声、伴奏、贝斯、和弦等）
- MIDI文件导出
- 无水印输出

### 5. 制作记录管理
- 历史项目保存
- 随时修改编辑
- 人声提取/替换
- 旋律参考对比

## 技术栈
- Framework: Next.js 16
- Language: TypeScript 5
- UI: shadcn/ui + Tailwind CSS 4
- Audio: Tone.js + Web Audio API
- AI: LLM流式生成

## 目录结构
```
src/
├── app/
│   ├── page.tsx                    # 首页
│   ├── layout.tsx                  # 主布局
│   ├── api/
│   │   ├── generate-music/route.ts # AI音乐生成
│   │   ├── analyze-audio/route.ts  # 音频分析
│   │   └── projects/route.ts       # 项目管理
│   ├── generate/                   # AI生成页面
│   ├── analyze/                    # 音频分析页面
│   ├── voice/                      # 变声器页面
│   └── projects/                   # 项目管理页面
├── components/
│   ├── audio/                      # 音频组件
│   ├── layout/                     # 布局组件
│   └── ui/                         # UI组件
└── lib/
    └── audio.ts                    # 音频处理工具
```

## 开发命令
- `pnpm dev` - 启动开发服务器
- `pnpm build` - 构建生产版本
- `pnpm start` - 启动生产服务器
