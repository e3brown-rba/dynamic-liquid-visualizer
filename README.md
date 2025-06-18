# Dynamic Liquid Audio Visualizer

Real-time audio visualization system featuring organic, liquid-like graphics that respond dynamically to system audio. Built with C#/.NET, OpenGL, and advanced audio processing techniques.

![Status: MVP Complete](https://img.shields.io/badge/Status-MVP%20Complete-green)
![Platform: Windows](https://img.shields.io/badge/Platform-Windows-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow)

## 🎯 Project Overview

This project demonstrates the intersection of technical program management and hands-on development, showcasing:
- **Real-time System Design**: Managing audio capture, processing, and rendering pipelines
- **Performance Optimization**: Achieving 60+ FPS while processing audio in real-time
- **User Experience**: Creating visually stunning, responsive graphics that enhance music enjoyment

## 🚀 Key Features

- **Organic Liquid Visualization**: Mercury-like fluid that pulses with bass and ripples with high frequencies
- **Real-time Audio Processing**: WASAPI loopback captures any system audio without configuration
- **Advanced Graphics Pipeline**: Custom GLSL shaders creating complex visual effects
- **Debug Visualization Modes**: 6 different modes for understanding audio-visual relationships
- **Zero-Configuration**: Works immediately with any audio playing on Windows

## 🛠️ Technical Stack

- **Language**: C# (.NET 8)
- **Graphics**: OpenGL 3.3+ via OpenTK
- **Audio**: NAudio (WASAPI Loopback)
- **Signal Processing**: FFT for frequency analysis
- **Shader Programming**: GLSL for GPU-accelerated effects

## 📊 Technical Achievements

### Performance Metrics
- Maintains 60+ FPS on mid-range hardware
- Sub-20ms audio-to-visual latency
- Efficient memory usage (~50MB)

### Audio Processing
- Real-time FFT with 1024-sample windows
- Frequency band separation (Bass/Mid/High)
- Adaptive level normalization

### Visual Innovation
- Metaball simulation for organic blob movement
- Multi-layer ripple system with decay
- Dynamic color temperature based on audio energy

## 🎮 Usage

### Quick Start
```bash
# Clone the repository
git clone https://github.com/yourusername/dynamic-liquid-visualizer.git

# Build and run
dotnet build
dotnet run --project DynamicLiquidVisualizer/DynamicLiquidVisualizer.csproj
```

### Controls
- `ESC` - Exit application
- `P` - Pause/Resume visualization
- `0-5` - Switch debug visualization modes
  - `0` - Normal (full liquid effect)
  - `1` - Blob visualization only
  - `2` - Ripple patterns only
  - `3` - Audio level meters
  - `4` - Surface normals
  - `5` - Matcap shading

## 🏗️ Architecture Highlights

### Modular Design
```
├── Audio/
│   ├── AudioCapture.cs      # System audio interception
│   └── AudioProcessor.cs    # FFT and frequency analysis
├── Graphics/
│   ├── Renderer.cs          # OpenGL pipeline management
│   └── Shaders/            # GLSL vertex/fragment shaders
└── Core/
    └── AppState.cs         # Centralized state management
```

### Key Design Decisions
- **Separation of Concerns**: Audio, graphics, and state management are fully decoupled
- **Error Resilience**: Graceful fallbacks if audio capture fails
- **Extensibility**: Easy to add new visualization modes or audio sources

## 💡 PM Perspective

This project showcases critical program management skills:

1. **Technical Leadership**: Making architectural decisions that balance performance, maintainability, and user experience
2. **Risk Management**: Implementing comprehensive error handling for audio/graphics subsystems
3. **Iterative Development**: MVP approach with clear enhancement pathway
4. **Cross-functional Skills**: Bridging audio engineering, graphics programming, and UX design

## 🔄 Future Enhancements

- [ ] Multi-platform support (macOS, Linux)
- [ ] Spotify API integration for track-specific visualizations
- [ ] VR/AR visualization modes
- [ ] Machine learning for genre-specific visual styles
- [ ] Plugin architecture for custom visualizations

## 📈 Business Applications

While built as a passion project, this demonstrates capabilities valuable for:
- **Gaming Industry**: Real-time audio integration for rhythm games or music-reactive environments
- **Live Events**: Visual installations for concerts or presentations  
- **Accessibility**: Audio visualization for hearing-impaired users
- **Data Visualization**: Techniques applicable to real-time business metrics

## 🤝 Contributing

This project is open for collaboration. Areas where contributions are welcome:
- Performance optimizations
- Additional visualization modes
- Cross-platform compatibility
- Documentation improvements

## 📜 License

MIT License - feel free to use this code in your own projects!

---

**Built by Eddy**  
Program Manager | Real-time Systems | Audio-Visual Innovation  
[LinkedIn](https://linkedin.com/in/eddy-brown) | [Email](mailto:e3brown@outlook.com)
