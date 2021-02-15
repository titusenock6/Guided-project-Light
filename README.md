//
//  ViewController.swift
//  Light
//
//  Created by Titus Enock on 2/15/21.
//

import UIKit

class ViewController: UIViewController {
    
    var lightOn = true

    @IBAction func buttonPressed(_ sender: Any) {
        lightOn = !lightOn
        upDateUI()
        
    }
    
    
    func upDateUI() {
        view.backgroundColor = lightOn ? .white : .black
        
    }
    override func viewDidLoad() {
        super.viewDidLoad()
        upDateUI()
        // Do any additional setup after loading the view.
    }


}
