import React, { useEffect, useMemo, useState } from "react";
import { motion } from "framer-motion";
import {
  CheckCircle2,
  CircleDollarSign,
  ClipboardList,
  Camera,
  Scissors,
  Rocket,
  Users,
  FileText,
  CalendarDays,
} from "lucide-react";

const pinkMascot = "https://aplen-chen.github.io/picture/IP.png";
const purpleMascot = "https://aplen-chen.github.io/picture/boyip.png";

const phases = [
  {
    title: "第一阶段：商务洽谈与确立合作",
    tag: "咨询期",
    steps: [
      {
        id: 1,
        node: "一次见面",
        left: { label: "Seko", text: "初步沟通，了解客户基本盘。", tone: "seko" },
        right: { label: "客人", text: "提出咨询需求。", tone: "client" },
        icon: Users,
      },
      {
        id: 2,
        node: "二次见面",
        left: { label: "Seko", text: "解答客户咨询，介绍公司情况，交付SOP陪跑细则。", tone: "seko" },
        right: { label: "客人", text: "深入了解公司与服务流程。", tone: "client" },
        icon: ClipboardList,
      },
      {
        id: 3,
        node: "三次见面",
        left: { label: "编导 / 负责人", text: "开始筹备项目。", tone: "team" },
        right: { label: "客户 / 负责人", text: "确认合作，完成付款。", tone: "client-strong" },
        icon: CircleDollarSign,
      },
    ],
  },
  {
    title: "第二阶段：账号定位与内容策划",
    tag: "筹备期",
    steps: [
      {
        id: 4,
        node: "付款后1天内",
        left: { label: "编导 + Seko", text: "内部准备与初步沟通。", tone: "team" },
        right: { label: "客户负责人", text: "参与沟通。", tone: "client" },
        icon: Users,
      },
      {
        id: 5,
        node: "7-14天内",
        left: { label: "编导", text: "独立输出账号策划表，定好4个选题。", tone: "team" },
        right: { label: "状态", text: "等待策划案", tone: "placeholder" },
        icon: FileText,
      },
      {
        id: 6,
        node: "付款后第2天左右",
        left: { label: "编导 + Seko", text: "主导会议，输出会议报告。", tone: "team" },
        right: { label: "客户负责人", text: "参会讨论并确认定位。", tone: "client" },
        icon: CalendarDays,
      },
      {
        id: 7,
        node: "1天内",
        left: { label: "编导", text: "输出初选题与剧本框架。", tone: "team" },
        right: { label: "客户", text: "提出修改跟进。", tone: "client" },
        icon: FileText,
      },
      {
        id: 8,
        node: "剧本定稿",
        center: { label: "双方共同", text: "共同确认剧本终稿。", tone: "center" },
        icon: CheckCircle2,
      },
    ],
  },
  {
    title: "第三阶段：拍摄执行",
    tag: "落地期",
    steps: [
      {
        id: 9,
        node: "剧本定稿后2天内",
        left: { label: "团队", text: "安排拍摄时间（需提前5天预约后面的时间）。", tone: "team" },
        right: { label: "客户", text: "确认档期配合。", tone: "client" },
        icon: CalendarDays,
      },
      {
        id: 10,
        node: "拍摄前1天内",
        left: { label: "拍摄与编导", text: "沟通剧本细节，安排拍摄人员。", tone: "team" },
        right: { label: "客户", text: "配合准备物料 / 状态。", tone: "client" },
        icon: Camera,
      },
      {
        id: 11,
        node: "拍摄当日",
        left: { label: "拍摄团队", text: "执行拍摄（通常3小时内完成5条剧本）。", tone: "team" },
        right: { label: "客户", text: "到场配合完成拍摄。", tone: "client" },
        icon: Camera,
      },
    ],
  },
  {
    title: "第四阶段：后期交付与发布",
    tag: "收尾期",
    steps: [
      {
        id: 12,
        node: "拍摄后1天内",
        left: { label: "拍摄", text: "上传素材并整理，通知剪辑和编导。", tone: "team" },
        icon: Scissors,
      },
      {
        id: 13,
        node: "素材整理后2天内",
        left: { label: "编导与剪辑", text: "沟通剧本剪辑细节；剪辑完成首条成片和模板。", tone: "team" },
        icon: Scissors,
      },
      {
        id: 14,
        node: "审片期",
        left: { label: "后期团队", text: "根据反馈修改（首条成片享受无限次修改，第2条开始2次 / 条修改）。", tone: "team" },
        right: { label: "客户", text: "审阅视频并提出修改意见。", tone: "client" },
        icon: FileText,
      },
      {
        id: 15,
        node: "发布期",
        left: { label: "编导", text: "给予发布文案，并做进度跟进提醒。", tone: "team" },
        right: { label: "客户", text: "发布首条影片。", tone: "client-strong" },
        icon: Rocket,
      },
      {
        id: 16,
        node: "完结",
        center: { label: "双方共同", text: "完成交付闭环。", tone: "center" },
        icon: CheckCircle2,
      },
    ],
  },
];

const allSteps = phases.flatMap((phase) =>
  phase.steps.map((step) => ({ ...step, phaseTitle: phase.title, phaseTag: phase.tag })),
);

const toneClass = {
  seko: "bg-blue-50 border-blue-300 text-blue-950",
  team: "bg-indigo-50 border-indigo-300 text-indigo-950",
  client: "bg-emerald-50 border-emerald-300 text-emerald-950",
  "client-strong": "bg-orange-50 border-orange-300 text-orange-950",
  placeholder: "bg-slate-50 border-slate-200 text-slate-500 border-dashed",
  center: "bg-gradient-to-r from-violet-500 via-fuchsia-500 to-cyan-500 text-white border-transparent",
};

function getProgress(activeStep) {
  if (!activeStep) return 0;
  return (activeStep / allSteps.length) * 100;
}

function runSanityChecks() {
  console.assert(allSteps.length === 16, "步骤总数应为16");
  console.assert(getProgress(8) === 50, "第8步进度应为50%");
  console.assert(getProgress(null) === 0, "未激活步骤时进度应为0");
}

runSanityChecks();

function MascotSprite({ src, label, side = "left", className = "" }) {
  return (
    <motion.div
      animate={{ y: [0, -8, 0] }}
      transition={{ duration: 4.5, repeat: Infinity, ease: "easeInOut" }}
      className={[
        "relative shrink-0 select-none",
        side === "left" ? "w-[150px] xl:w-[170px]" : "w-[132px] xl:w-[152px]",
        className,
      ].join(" ")}
    >
      <div className="absolute inset-0 rounded-full bg-gradient-to-b from-pink-200/25 via-violet-200/15 to-transparent blur-3xl" />
      <img
        src={src}
        alt={label}
        className="relative z-10 block h-auto w-full object-contain bg-transparent mix-blend-multiply drop-shadow-[0_20px_35px_rgba(99,102,241,0.14)]"
      />
    </motion.div>
  );
}

function HeroSection() {
  return (
    <header className="relative mb-10 overflow-hidden rounded-[36px] border border-white/80 bg-white/80 px-6 py-10 shadow-[0_22px_80px_rgba(15,23,42,0.08)] backdrop-blur md:px-8 lg:px-12 lg:py-14">
      <div className="absolute inset-0 bg-[radial-gradient(circle_at_15%_30%,rgba(59,130,246,0.08),transparent_24%),radial-gradient(circle_at_80%_20%,rgba(244,114,182,0.08),transparent_18%),radial-gradient(circle_at_50%_100%,rgba(16,185,129,0.06),transparent_22%)]" />

      <div className="relative flex min-h-[180px] items-center justify-center">
        <div className="pointer-events-none absolute left-0 top-1/2 hidden -translate-y-1/2 xl:block">
          <MascotSprite src={pinkMascot} label="女IP角色" side="left" />
        </div>

        <div className="pointer-events-none absolute right-0 top-1/2 hidden -translate-y-1/2 xl:block">
          <MascotSprite src={purpleMascot} label="男IP角色" side="right" />
        </div>

        <div className="relative z-10 text-center">
          <div className="mx-auto h-px w-24 bg-gradient-to-r from-transparent via-slate-300 to-transparent" />
          <h1 className="mt-5 text-3xl font-black tracking-tight text-slate-950 md:text-5xl xl:text-[56px] xl:leading-[1.08]">
            <span>客户咨询与业务交付</span>
            <span className="ml-3 inline bg-gradient-to-r from-blue-600 via-indigo-600 to-violet-500 bg-clip-text text-transparent">
              SOP流程图
            </span>
          </h1>
          <div className="mx-auto mt-6 h-px w-24 bg-gradient-to-r from-transparent via-slate-300 to-transparent" />
        </div>
      </div>
    </header>
  );
}

function Card({ item, active, muted, align = "left" }) {
  if (!item) return <div className="hidden lg:block" />;

  const isCenter = item.tone === "center";

  return (
    <div
      className={[
        "group relative rounded-3xl border p-4 md:p-5 shadow-[0_10px_30px_rgba(15,23,42,0.08)] transition-all duration-300",
        toneClass[item.tone],
        active ? "scale-[1.02] shadow-[0_20px_50px_rgba(59,130,246,0.22)] ring-2 ring-white/70" : "",
        muted ? "opacity-35 saturate-50" : "opacity-100",
        align === "left" ? "lg:mr-10" : "lg:ml-10",
        isCenter ? "overflow-hidden" : "backdrop-blur-sm",
      ].join(" ")}
    >
      {isCenter ? (
        <div className="absolute inset-0 bg-[radial-gradient(circle_at_top_right,rgba(255,255,255,0.35),transparent_36%)]" />
      ) : null}

      <div className="relative z-10 flex items-start justify-between gap-3">
        <div>
          <div
            className={`mb-2 inline-flex rounded-full px-3 py-1 text-xs font-semibold tracking-[0.14em] ${
              isCenter ? "bg-white/20 text-white" : "bg-white/70 text-slate-700"
            }`}
          >
            {item.label}
          </div>
          <p className={`text-sm leading-6 md:text-[15px] ${isCenter ? "text-white/95" : "text-slate-700"}`}>
            {item.text}
          </p>
        </div>
      </div>
    </div>
  );
}

function StepRow({ step, index, activeStep, setActiveStep }) {
  const isActive = activeStep === step.id;
  const isMuted = activeStep !== null && activeStep !== step.id;
  const Icon = step.icon || CircleDollarSign;

  return (
    <motion.div
      initial={{ opacity: 0, y: 30 }}
      whileInView={{ opacity: 1, y: 0 }}
      viewport={{ once: true, amount: 0.25 }}
      transition={{ duration: 0.45, delay: index * 0.03 }}
      className="relative"
      onMouseEnter={() => setActiveStep(step.id)}
      onMouseLeave={() => setActiveStep(null)}
    >
      <div
        className={[
          "relative grid items-center gap-5 lg:grid-cols-[minmax(0,1fr)_120px_minmax(0,1fr)]",
          activeStep !== null && activeStep !== step.id ? "opacity-55" : "opacity-100",
        ].join(" ")}
      >
        {!step.center ? (
          <motion.div
            initial={{ opacity: 0, x: -36 }}
            whileInView={{ opacity: 1, x: 0 }}
            viewport={{ once: true, amount: 0.35 }}
            transition={{ duration: 0.45, delay: 0.04 }}
            className="relative"
          >
            <Card item={step.left} active={isActive} muted={isMuted} align="left" />
          </motion.div>
        ) : (
          <div className="hidden lg:block" />
        )}

        <div className="relative flex min-h-[110px] items-center justify-center lg:min-h-[144px]">
          <div
            className={`absolute left-1/2 top-0 h-full w-1.5 -translate-x-1/2 rounded-full transition-all duration-300 ${
              isActive
                ? "bg-gradient-to-b from-cyan-400 via-blue-500 to-violet-500 shadow-[0_0_28px_rgba(59,130,246,0.45)]"
                : "bg-slate-300"
            }`}
          />

          {step.left && !step.center ? (
            <div className="pointer-events-none absolute left-[calc(50%-240px)] right-1/2 top-1/2 hidden -translate-y-1/2 lg:block">
              <div
                className={`relative h-px border-t-2 border-dashed transition-all duration-300 ${
                  isActive ? "border-blue-500" : "border-slate-300"
                }`}
              >
                <div
                  className={`absolute -right-1 -top-[5px] h-0 w-0 border-b-[6px] border-l-[9px] border-t-[6px] border-b-transparent border-t-transparent ${
                    isActive ? "border-l-blue-500" : "border-l-slate-300"
                  }`}
                />
              </div>
            </div>
          ) : null}

          {step.right && !step.center ? (
            <div className="pointer-events-none absolute left-1/2 right-[calc(50%-240px)] top-1/2 hidden -translate-y-1/2 lg:block">
              <div
                className={`relative h-px border-t-2 border-dashed transition-all duration-300 ${
                  isActive ? "border-emerald-500" : "border-slate-300"
                }`}
              >
                <div
                  className={`absolute -left-1 -top-[5px] h-0 w-0 border-b-[6px] border-r-[9px] border-t-[6px] border-b-transparent border-t-transparent ${
                    isActive ? "border-r-emerald-500" : "border-r-slate-300"
                  }`}
                />
              </div>
            </div>
          ) : null}

          <div
            className={`relative z-10 flex h-20 w-20 flex-col items-center justify-center rounded-full border-4 bg-white p-2 text-center shadow-lg transition-all duration-300 ${
              isActive ? "scale-110 border-blue-500 shadow-[0_0_35px_rgba(59,130,246,0.28)]" : "border-slate-300"
            }`}
          >
            <Icon className={`mb-1 h-4 w-4 ${isActive ? "text-blue-600" : "text-slate-500"}`} />
            <span className="text-[10px] font-bold tracking-[0.14em] text-slate-500">STEP {step.id}</span>
          </div>

          <div className="absolute left-1/2 top-full mt-3 w-28 -translate-x-1/2 text-center text-xs font-medium leading-5 text-slate-500 md:w-36">
            {step.node}
          </div>
        </div>

        {!step.center ? (
          <motion.div
            initial={{ opacity: 0, x: 36 }}
            whileInView={{ opacity: 1, x: 0 }}
            viewport={{ once: true, amount: 0.35 }}
            transition={{ duration: 0.45, delay: 0.04 }}
            className="relative"
          >
            <Card item={step.right} active={isActive} muted={isMuted} align="right" />
          </motion.div>
        ) : (
          <div className="hidden lg:block" />
        )}

        {step.center ? (
          <div className="pointer-events-none absolute inset-x-0 top-1/2 hidden -translate-y-1/2 justify-center lg:flex">
            <div className="w-[min(36rem,58vw)]">
              <Card item={step.center} active={isActive} muted={isMuted} align="center" />
            </div>
          </div>
        ) : null}
      </div>

      <div className="mt-10 space-y-3 lg:hidden">
        {step.center ? (
          <Card item={step.center} active={isActive} muted={isMuted} align="center" />
        ) : (
          <>
            <div className="ml-8 border-l border-dashed border-blue-200 pl-5">
              <Card item={step.left} active={isActive} muted={isMuted} align="left" />
            </div>
            {step.right ? (
              <div className="ml-8 border-l border-dashed border-emerald-200 pl-5">
                <Card item={step.right} active={isActive} muted={isMuted} align="right" />
              </div>
            ) : null}
          </>
        )}
      </div>
    </motion.div>
  );
}

export default function SopTimelineLadderPage() {
  const [activeStep, setActiveStep] = useState(null);
  const progress = useMemo(() => getProgress(activeStep), [activeStep]);

  useEffect(() => {
    const onLeave = () => setActiveStep(null);
    window.addEventListener("scroll", onLeave, { passive: true });
    return () => window.removeEventListener("scroll", onLeave);
  }, []);

  return (
    <div className="min-h-screen bg-slate-50 text-slate-900">
      <div className="absolute inset-0 bg-[radial-gradient(circle_at_top,rgba(59,130,246,0.10),transparent_32%),radial-gradient(circle_at_bottom_right,rgba(16,185,129,0.08),transparent_22%)]" />

      <div className="relative mx-auto max-w-7xl px-4 py-10 md:px-6 lg:px-8 lg:py-14">
        <HeroSection />

        <section className="relative overflow-hidden rounded-[36px] border border-slate-200 bg-white px-4 py-8 shadow-[0_20px_80px_rgba(15,23,42,0.08)] md:px-6 lg:px-10 lg:py-12">
          <div className="pointer-events-none absolute left-0 right-0 top-0 h-40 bg-gradient-to-b from-blue-50/70 via-white/0 to-transparent" />

          <div className="mb-8 flex items-center justify-between gap-4 rounded-3xl border border-slate-200 bg-slate-50 px-4 py-4 md:px-5">
            <div>
              <h2 className="text-xl font-black tracking-tight text-slate-900 md:text-2xl">流程图</h2>
              <p className="mt-1 text-sm text-slate-500">从咨询确认到交付完结的完整路径</p>
            </div>
            <div className="hidden items-center gap-5 text-sm font-semibold text-slate-500 lg:flex">
              <div className="flex items-center gap-2">
                <span className="h-2.5 w-2.5 rounded-full bg-blue-500" />公司团队
              </div>
              <div className="flex items-center gap-2">
                <span className="h-2.5 w-2.5 rounded-full bg-slate-400" />时间轴
              </div>
              <div className="flex items-center gap-2">
                <span className="h-2.5 w-2.5 rounded-full bg-emerald-500" />客户
              </div>
            </div>
          </div>

          <div className="mb-10 rounded-3xl border border-slate-200 bg-slate-50 p-4 md:p-5">
            <div className="mb-2 flex items-center justify-between text-xs font-semibold tracking-[0.16em] text-slate-500">
              <span>时间进度</span>
              <span>{activeStep ? `STEP ${activeStep} / 16` : "悬停步骤查看联动"}</span>
            </div>
            <div className="h-3 overflow-hidden rounded-full bg-slate-200">
              <div
                className="h-full rounded-full bg-gradient-to-r from-blue-500 via-indigo-500 to-emerald-500 transition-all duration-500"
                style={{ width: `${progress}%` }}
              />
            </div>
          </div>

          <div className="space-y-12 lg:space-y-16">
            {phases.map((phase, phaseIndex) => (
              <div key={phase.title} className="relative">
                <div className="sticky top-4 z-20 mb-8 flex justify-center lg:mb-10">
                  <div className="rounded-full border border-slate-200 bg-white/95 px-5 py-2.5 shadow-lg backdrop-blur">
                    <span className="mr-3 text-xs font-black tracking-[0.18em] text-slate-400">0{phaseIndex + 1}</span>
                    <span className="text-sm font-bold text-slate-800">{phase.title}</span>
                    <span className="ml-3 rounded-full bg-slate-100 px-2.5 py-1 text-xs font-semibold text-slate-500">
                      {phase.tag}
                    </span>
                  </div>
                </div>

                <div className="space-y-10 lg:space-y-14">
                  {phase.steps.map((step, stepIndex) => (
                    <StepRow
                      key={step.id}
                      step={step}
                      index={stepIndex}
                      activeStep={activeStep}
                      setActiveStep={setActiveStep}
                    />
                  ))}
                </div>
              </div>
            ))}
          </div>
        </section>
      </div>
    </div>
  );
}
