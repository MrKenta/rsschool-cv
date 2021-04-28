## rsschool-cv

### RAMAN KRUTSIOU

### Contact Info

1. E-mail: mrsaiti14@icloud.com
2. Mobile: +375(33)647-92-45


## Summary 

My main goal is to improve my skills and knowledge in iOS.

## Skills

1. Swift
2. Objective - C

## Code examples

import Foundation

class Download {

    var stringURL = ""
    
    func downloader(completion: @escaping (Data) -> Void) {
        guard let fileManager = Bundle.main.path(forResource:"URL", ofType:"txt") else { return }
        do{
            let content = try! String(contentsOfFile: fileManager)
            stringURL = content
        }
        
        guard let url = URL(string: stringURL.trimmingCharacters(in: .whitespacesAndNewlines)) else { return }
        let session = URLSession.shared
        session.dataTask(with: url) { (data, response, error) in
            guard let dataImage = data else { return }
            completion(dataImage)
        }.resume()
        
    }
}

## Education 

### Belarusian National Technical University

MECHANICAL ENGINEERING TECHNOLOGY  2014 - 2019

### Teach Me Skills 

iOS Development


## English

Pre-intermediate +



