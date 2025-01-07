# Visio2000-BasicNetworkShapes3D
 Basic Network Shapes 3D stencils from Visio 2000 to PlantUML sprites.

 The VSS stencil to SVG/PNG conversion process has been documented [here](https://translate.google.com/translate?sl=pt&tl=en&hl=pt-BR&u=https://eduardomozartdeoliveira.wordpress.com/2023/01/30/instalacao-do-libvisio2svg-no-macos/).

 ## Samples

![Sample](Sample.png)

### Network Diagram

![Basic Usage - Certificate Authority](https://www.plantuml.com/plantuml/png/nPDFRzD04CNl-occLM-8s4tXOeMeRNeCLKMWGi883TvfCifwrjgT9VnHlpiRsmV-5C41mi7h9-_p_6RUskTHCMXgdObRbWu3jc3f3fFJb_HHBnolfILHQF92mPYZlCj2SCkH_NHxJGeRrIvMHH5mDrcpRjBx52aqNfH49url2x89W_Mj_vnXnV1gMPQFBp5oaqliVDYkDjXHFBigMcGnHooDI_PRJj7bDeiLXGyK9dlzQzCDXUW5tRiCxvB-rh_4JdqtcCmiwYT7SoCxoxY-ojS-b2y68FRiNW9SOhDT1v_4Bhpp0SGBzHjB5lhXKLxkpRsP5MFfiNPVwIwMf_36Kcm2TyfUu1aSpruzAijfEVzlzvCXvtajUy7MXmfMBsxBqrfkC2h2Fja9LB2ewkSe2JdMii2MPUChgEl1E-uSlpK6G8PpXkN5zHZXCFme6ySa-b0M9pyTPsuB5hsVilhJeLvNkP7lODC7OCEtyBS8PuSSvyaXOK__CMpuPSv9R6hTLm00)

```csharp
@startuml
skinparam defaultTextAlignment center

!define Visio2kNet https://raw.githubusercontent.com/eduardomozart/Visio2000-BasicNetworkShapes3D/main
!include Visio2kNet/puml/Server.puml
!include Visio2kNet/puml/Personal_computer.puml
!include Visio2kNet/puml/Laptop.puml

<style>
nwdiagDiagram {
  server {
    BackgroundColor none
    LineColor none
    
  }
}
</style>

nwdiag {
  fs01 [description = "<U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><U+0020><$Server>\nServidor: SRV01\nPasta comp. : C:\Manuais\nCaminho: \\SRV01\Manuais"]

  network LAN {
      fs01
      client01 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client02 [description = "<$Laptop>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client03 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client04 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
      client05 [description = "<$Personal_computer>\n Cliente\n <U+0020><U+0020><U+0020><U+0020><U+0020>X:"]
  }
}
@enduml
```