import { Card } from "@/components/ui/card"
import { Badge } from "@/components/ui/badge"
import { Button } from "@/components/ui/button"
import { GithubIcon, TwitterIcon, LinkedinIcon, InstagramIcon, MailIcon } from "lucide-react"

export default function Component() {
  return (
    <div className="bg-[#0d1117] p-6 min-h-screen text-white font-sans">
      <div className="max-w-4xl mx-auto space-y-6">
        {/* Intro Section */}
        <Card className="bg-white p-0.5 rounded-lg overflow-hidden">
          <div className="bg-[#0d1117] p-6 rounded-lg">
            <img
              src="/placeholder.svg?height=200&width=800"
              alt="Jorge Alejandro Diez"
              className="w-full rounded-lg mb-6"
            />
            <h1 className="text-3xl font-bold text-[#58a6ff] mb-2">
              👋 Hello, I'm Jorge Alejandro Diez
            </h1>
            <p className="text-xl text-[#58a6ff] mb-4">
              Web Developer | AI Enthusiast | Data Visualization Specialist
            </p>
            <div className="flex flex-wrap gap-2 mb-6">
              <Badge variant="secondary"><TwitterIcon className="w-4 h-4 mr-1" /> Twitter</Badge>
              <Badge variant="secondary"><LinkedinIcon className="w-4 h-4 mr-1" /> LinkedIn</Badge>
              <Badge variant="secondary"><GithubIcon className="w-4 h-4 mr-1" /> GitHub</Badge>
            </div>
            <h2 className="text-2xl font-semibold text-[#58a6ff] mb-4">🚀 About Me</h2>
            <p className="text-[#c9d1d9] mb-4">
              I'm a passionate web developer early in my career, driven by a commitment to excellence and innovation...
            </p>
            <div className="grid grid-cols-2 gap-4">
              <div className="flex items-center">
                <img src="/placeholder.svg?height=24&width=24" className="w-6 h-6 mr-2" alt="AI icon" />
                <span className="text-[#c9d1d9]">Working on <strong className="text-[#58a6ff]">AI Object Detection Model for Football</strong></span>
              </div>
              <div className="flex items-center">
                <img src="/placeholder.svg?height=24&width=24" className="w-6 h-6 mr-2" alt="Learn icon" />
                <span className="text-[#c9d1d9]">Learning <strong className="text-[#58a6ff]">AI, Data Science, Data Visualization</strong></span>
              </div>
            </div>
          </div>
        </Card>

        {/* Skills Section */}
        <Card className="bg-white p-0.5 rounded-lg overflow-hidden">
          <div className="bg-[#0d1117] p-6 rounded-lg">
            <h2 className="text-2xl font-semibold text-[#58a6ff] mb-4">💼 Skills & Tools</h2>
            <div className="flex flex-wrap gap-2 mb-4">
              <Badge>AWS</Badge>
              <Badge>React</Badge>
              <Badge>Vue.js</Badge>
              <Badge>JavaScript</Badge>
              <Badge>Python</Badge>
              <Badge>Docker</Badge>
              <Badge>TensorFlow</Badge>
            </div>
            <Button variant="outline" className="w-full">View full list of technologies and tools</Button>
          </div>
        </Card>

        {/* GitHub Stats Section */}
        <Card className="bg-white p-0.5 rounded-lg overflow-hidden">
          <div className="bg-[#0d1117] p-6 rounded-lg">
            <h2 className="text-2xl font-semibold text-[#58a6ff] mb-4">📊 GitHub Stats</h2>
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
              <img src="/placeholder.svg?height=200&width=400" alt="GitHub stats" className="w-full rounded-lg" />
              <img src="/placeholder.svg?height=200&width=400" alt="GitHub streak" className="w-full rounded-lg" />
            </div>
          </div>
        </Card>

        {/* Featured Projects Section */}
        <Card className="bg-white p-0.5 rounded-lg overflow-hidden">
          <div className="bg-[#0d1117] p-6 rounded-lg">
            <h2 className="text-2xl font-semibold text-[#58a6ff] mb-4">🚀 Featured Projects</h2>
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
              <Card className="bg-[#161b22] p-4 rounded-lg">
                <img src="/placeholder.svg?height=150&width=300" alt="AI Football Analyzer" className="w-full rounded-lg mb-2" />
                <h3 className="text-lg font-semibold text-[#58a6ff] mb-2">AI Football Analyzer</h3>
                <p className="text-sm text-[#8b949e] mb-2">An AI-powered tool for analyzing football matches and player performance.</p>
                <Button size="sm">View Project</Button>
              </Card>
              <Card className="bg-[#161b22] p-4 rounded-lg">
                <img src="/placeholder.svg?height=150&width=300" alt="Data Viz Dashboard" className="w-full rounded-lg mb-2" />
                <h3 className="text-lg font-semibold text-[#58a6ff] mb-2">Data Viz Dashboard</h3>
                <p className="text-sm text-[#8b949e] mb-2">Interactive data visualization dashboard for complex datasets.</p>
                <Button size="sm">View Project</Button>
              </Card>
            </div>
          </div>
        </Card>

        {/* Contact Section */}
        <Card className="bg-white p-0.5 rounded-lg overflow-hidden">
          <div className="bg-[#0d1117] p-6 rounded-lg">
            <h2 className="text-2xl font-semibold text-[#58a6ff] mb-4">📫 Get in Touch</h2>
            <div className="flex flex-wrap gap-2 mb-4">
              <Badge variant="secondary"><MailIcon className="w-4 h-4 mr-1" /> Email</Badge>
              <Badge variant="secondary"><LinkedinIcon className="w-4 h-4 mr-1" /> LinkedIn</Badge>
              <Badge variant="secondary"><TwitterIcon className="w-4 h-4 mr-1" /> Twitter</Badge>
              <Badge variant="secondary"><InstagramIcon className="w-4 h-4 mr-1" /> Instagram</Badge>
            </div>
            <div className="flex gap-4">
              <Button>Visit my website</Button>
              <Button>Read my blog</Button>
            </div>
          </div>
        </Card>

        <div className="text-center text-sm text-[#8b949e] mt-8">
          © 2023 Jorge Alejandro Diez. All rights reserved.
        </div>
      </div>
    </div>
  )
}
