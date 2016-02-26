# university-Intranet
An University Intranet, for a project in J2EE

# DB :


    --
    -- Table structure for table `administrateur`
    --
    
    CREATE TABLE `administrateur` (
      `id` int(11) NOT NULL,
      `nom` varchar(200) NOT NULL,
      `prenom` varchar(200) NOT NULL,
      `email` varchar(200) NOT NULL,
      `civilite` varchar(200) DEFAULT NULL,
      `addresse` varchar(1000) DEFAULT NULL,
      `telephone` varchar(200) DEFAULT NULL,
      `motdepasse` varchar(200) NOT NULL
    ) ENGINE=InnoDB DEFAULT CHARSET=utf8;
    
    -- --------------------------------------------------------
    
    --
    -- Table structure for table `enseignant`
    --
    
    CREATE TABLE `enseignant` (
      `id` int(11) NOT NULL,
      `nom` varchar(200) NOT NULL,
      `prenom` varchar(200) NOT NULL,
      `email` varchar(200) NOT NULL,
      `civilite` varchar(200) DEFAULT NULL,
      `addresse` varchar(1000) DEFAULT NULL,
      `telephone` varchar(200) DEFAULT NULL,
      `motdepasse` varchar(200) NOT NULL
    ) ENGINE=InnoDB DEFAULT CHARSET=utf8;
    
    -- --------------------------------------------------------
    
    --
    -- Table structure for table `etudiant`
    --
    
    CREATE TABLE `etudiant` (
      `id` int(11) NOT NULL,
      `nom` varchar(200) NOT NULL,
      `prenom` varchar(200) NOT NULL,
      `email` varchar(200) NOT NULL,
      `classe` varchar(200) NOT NULL,
      `civilite` varchar(200) DEFAULT NULL,
      `adresse` varchar(1000) DEFAULT NULL,
      `telephone` varchar(200) DEFAULT NULL,
      `motdepasse` varchar(200) NOT NULL
    ) ENGINE=InnoDB DEFAULT CHARSET=utf8;
    
    --
    -- Dumping data for table `etudiant`
    --
    
    INSERT INTO `etudiant` (`id`, `nom`, `prenom`, `email`, `classe`, `civilite`, `adresse`, `telephone`, `motdepasse`) VALUES
    (1, 'theron', 'loup', 'test@test.com', '3CI', 'Mr', '151, rue du test', '0685694455', 'encoreuntest');
    
    --
    -- Indexes for table `administrateur`
    --
    ALTER TABLE `administrateur`
      ADD PRIMARY KEY (`id`);
    
    --
    -- Indexes for table `enseignant`
    --
    ALTER TABLE `enseignant`
      ADD PRIMARY KEY (`id`);
    
    --
    -- Indexes for table `etudiant`
    --
    ALTER TABLE `etudiant`
      ADD PRIMARY KEY (`id`);
    
    -- AUTO_INCREMENT for table `administrateur`
    --
    ALTER TABLE `administrateur`
      MODIFY `id` int(11) NOT NULL AUTO_INCREMENT;
    --
    -- AUTO_INCREMENT for table `enseignant`
    --
    ALTER TABLE `enseignant`
      MODIFY `id` int(11) NOT NULL AUTO_INCREMENT;
    --
    -- AUTO_INCREMENT for table `etudiant`
    --
    ALTER TABLE `etudiant`
      MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=2;
